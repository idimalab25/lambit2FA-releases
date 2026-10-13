lambit2FA Linuxille — versio 1.1

Kaksivaiheisen kirjautumisen koodit omalla tietokoneellasi. Ei tiliä, ei internetiä. Koodit tallennetaan salattuina; avain on järjestelmän avainnipussa (GNOME Keyring tai KWallet) tai, jos sellaista ei ole, tiedostossa, joka on sidottu tähän tietokoneeseen ja käyttäjääsi.

Tavallisille tietokoneille (Intel tai AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

ARM-tietokoneille (Raspberry Pi 4/5, virtuaalikoneet Apple Siliconilla, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

Käynnistys: 1. Lataa tiedosto. 2. Salli suoritus: oikea painike → Ominaisuudet → ”Salli tiedoston suorittaminen ohjelmana”, tai päätteessä: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Avaa se. Mitään ei asenneta — sovellus on yksi tiedosto. Poistaaksesi sen poista tiedosto; koodit säilyvät kansiossa ~/.config/lambit2FA.

Toimii Ubuntu 22.04:ssä ja uudemmissa, Debian 12:ssa ja uudemmissa, Linux Mint 21:ssä ja uudemmissa, Pop!_OS 22.04:ssä ja uudemmissa, Fedora 38:ssa ja uudemmissa. Muita jakeluja ei ole testattu. Jos tiedosto ei avaudu, asenna libfuse2: sudo apt install libfuse2 (Ubuntu 24.04: libfuse2t64).

Ensimmäisellä käynnistyksellä järjestelmä voi kysyä ”login”-avainnipun salasanaa. Kysyjä on järjestelmä, ei sovellus: sovellus tallettaa avaimensa järjestelmän avainnippuun. Anna avainnipun salasana tai paina Peruuta — silloin avain pidetään tiedostossa, joka on sidottu tähän tietokoneeseen ja käyttäjääsi.

QR-koodin lukeminen näytöltä vaatii Waylandissa kuvakaappaustyökalun (gnome-screenshot, spectacle tai grim). Ilman sitä ota kuvakaappaus itse ja avaa se sovelluksessa kuvana.

Latauksen tarkistus: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — tuloksen pitää vastata viereistä .sha256-tiedostoa.
