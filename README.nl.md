lambit2FA voor Linux — versie 1.1

Codes voor tweestapsaanmelding op uw computer. Geen account en geen internet nodig. De codes worden versleuteld bewaard; de sleutel staat in de sleutelbos van het systeem (GNOME Keyring of KWallet) of, waar die ontbreekt, in een bestand dat aan deze computer en uw gebruiker is gekoppeld.

Voor gewone computers (Intel of AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

Voor ARM-computers (Raspberry Pi 4/5, virtuele machines op Apple Silicon, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

Zo start u: 1. Download het bestand. 2. Sta uitvoeren toe: rechtsklik → Eigenschappen → “Uitvoeren van bestand als programma toestaan”, of in een terminal: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Open het. Er wordt niets geïnstalleerd — de app is één bestand. Verwijderen: wis het bestand; uw codes blijven in ~/.config/lambit2FA.

Werkt op Ubuntu 22.04 en nieuwer, Debian 12 en nieuwer, Linux Mint 21 en nieuwer, Pop!_OS 22.04 en nieuwer, Fedora 38 en nieuwer. Andere distributies zijn niet getest. Opent het bestand niet, installeer dan libfuse2: sudo apt install libfuse2 (op Ubuntu 24.04: libfuse2t64).

Bij de eerste start kan het systeem om het wachtwoord van de sleutelbos “login” vragen. Dat vraagt het systeem, niet de app: de app legt zijn sleutel in de sleutelbos van het systeem. Voer het wachtwoord van de sleutelbos in of druk op Annuleren — dan wordt de sleutel bewaard in een bestand dat aan deze computer en uw gebruiker is gekoppeld.

Een QR-code van het scherm lezen vereist op Wayland een schermafbeeldingsprogramma (gnome-screenshot, spectacle of grim). Zonder dat maakt u zelf een schermafbeelding en opent u die in de app als afbeelding.

Download controleren: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — de uitkomst moet overeenkomen met het .sha256-bestand ernaast.
