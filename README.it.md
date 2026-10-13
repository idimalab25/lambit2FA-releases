lambit2FA per Linux — versione 1.1

Codici di accesso a due fattori sul tuo computer. Senza account e senza Internet. I codici sono salvati cifrati; la chiave sta nel portachiavi di sistema (GNOME Keyring o KWallet) oppure, dove non c’è, in un file legato a questo computer e al tuo utente.

Per i computer comuni (Intel o AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

Per i computer ARM (Raspberry Pi 4/5, macchine virtuali su Apple Silicon, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

Come avviare: 1. Scarica il file. 2. Consenti l’esecuzione: tasto destro → Proprietà → «Consenti l’esecuzione del file come programma», oppure nel terminale: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Aprilo. Non si installa nulla: l’app è un solo file. Per rimuoverla, elimina il file; i codici restano in ~/.config/lambit2FA.

Funziona su Ubuntu 22.04 e successivi, Debian 12 e successivi, Linux Mint 21 e successivi, Pop!_OS 22.04 e successivi, Fedora 38 e successivi. Le altre distribuzioni non sono testate. Se il file non si apre, installa libfuse2: sudo apt install libfuse2 (su Ubuntu 24.04: libfuse2t64).

Al primo avvio il sistema può chiedere la password del portachiavi «login». A chiedere è il sistema, non l’app: l’app mette la sua chiave nel portachiavi di sistema. Inserisci la password del portachiavi oppure premi Annulla: la chiave verrà allora tenuta in un file legato a questo computer e al tuo utente.

Per leggere un codice QR dallo schermo su Wayland serve uno strumento per gli screenshot (gnome-screenshot, spectacle o grim). Senza, fai tu lo screenshot e aprilo nell’app come immagine.

Verifica del download: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — il risultato deve coincidere con il file .sha256 accanto.
