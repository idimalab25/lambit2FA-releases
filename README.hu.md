lambit2FA Linuxra — 1.1-es verzió

Kétlépcsős bejelentkezési kódok a saját gépén. Nem kell fiók, nem kell internet. A kódok titkosítva tárolódnak; a kulcs a rendszer kulcstartójában (GNOME Keyring vagy KWallet) van, ahol pedig nincs ilyen, egy ehhez a géphez és az Ön felhasználójához kötött fájlban.

Hagyományos számítógépekre (Intel vagy AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

ARM-számítógépekre (Raspberry Pi 4/5, virtuális gépek Apple Siliconon, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

Indítás: 1. Töltse le a fájlt. 2. Engedélyezze a futtatást: jobb kattintás → Tulajdonságok → „Fájl futtatásának engedélyezése programként”, vagy terminálban: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Nyissa meg. Semmi sem települ — az app egyetlen fájl. Eltávolításhoz törölje a fájlt; a kódok a ~/.config/lambit2FA mappában maradnak.

Működik Ubuntu 22.04 és újabb, Debian 12 és újabb, Linux Mint 21 és újabb, Pop!_OS 22.04 és újabb, Fedora 38 és újabb rendszereken. Más disztribúciók nincsenek kipróbálva. Ha a fájl nem nyílik meg, telepítse a libfuse2-t: sudo apt install libfuse2 (Ubuntu 24.04-en: libfuse2t64).

Az első indításkor a rendszer kérheti a „login” kulcstartó jelszavát. A rendszer kérdez, nem az app: az app a saját kulcsát a rendszer kulcstartójába teszi. Adja meg a kulcstartó jelszavát, vagy nyomja meg a Mégse gombot — ekkor a kulcs egy ehhez a géphez és az Ön felhasználójához kötött fájlban marad.

QR-kód képernyőről olvasásához Waylanden képernyőkép-eszköz kell (gnome-screenshot, spectacle vagy grim). Enélkül készítsen képernyőképet maga, és nyissa meg az appban képként.

A letöltés ellenőrzése: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — az eredménynek egyeznie kell a mellette lévő .sha256 fájllal.
