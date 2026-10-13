lambit2FA pentru Linux — versiunea 1.1

Coduri de autentificare în doi pași pe calculatorul dvs. Fără cont și fără internet. Codurile sunt păstrate criptate; cheia stă în inelul de chei al sistemului (GNOME Keyring sau KWallet) sau, unde nu există, într-un fișier legat de acest calculator și de utilizatorul dvs.

Pentru calculatoare obișnuite (Intel sau AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

Pentru calculatoare ARM (Raspberry Pi 4/5, mașini virtuale pe Apple Silicon, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

Cum se pornește: 1. Descărcați fișierul. 2. Permiteți rularea: clic dreapta → Proprietăți → „Permite executarea fișierului ca program”, sau în terminal: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Deschideți-l. Nu se instalează nimic — aplicația este un singur fișier. Pentru a o elimina, ștergeți fișierul; codurile rămân în ~/.config/lambit2FA.

Funcționează pe Ubuntu 22.04 și mai nou, Debian 12 și mai nou, Linux Mint 21 și mai nou, Pop!_OS 22.04 și mai nou, Fedora 38 și mai nou. Alte distribuții nu au fost testate. Dacă fișierul nu se deschide, instalați libfuse2: sudo apt install libfuse2 (pe Ubuntu 24.04: libfuse2t64).

La prima pornire sistemul poate cere parola inelului de chei „login”. Întreabă sistemul, nu aplicația: aplicația își pune cheia în inelul de chei al sistemului. Introduceți parola inelului sau apăsați Anulare — atunci cheia va fi păstrată într-un fișier legat de acest calculator și de utilizatorul dvs.

Citirea unui cod QR de pe ecran pe Wayland are nevoie de un instrument de captură (gnome-screenshot, spectacle sau grim). Fără el, faceți captura singur și deschideți-o în aplicație ca imagine.

Verificarea descărcării: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — rezultatul trebuie să coincidă cu fișierul .sha256 de alături.
