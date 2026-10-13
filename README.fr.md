lambit2FA pour Linux — version 1.1

Codes de connexion à deux facteurs sur votre ordinateur. Sans compte et sans Internet. Les codes sont stockés chiffrés ; la clé se trouve dans le trousseau du système (GNOME Keyring ou KWallet) ou, à défaut, dans un fichier lié à cet ordinateur et à votre utilisateur.

Pour les ordinateurs ordinaires (Intel ou AMD, x86_64) :
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

Pour les ordinateurs ARM (Raspberry Pi 4/5, machines virtuelles sur Apple Silicon, aarch64) :
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

Pour lancer : 1. Téléchargez le fichier. 2. Autorisez son exécution : clic droit → Propriétés → « Autoriser l'exécution du fichier comme un programme », ou dans un terminal : chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Ouvrez-le. Rien n'est installé — l'application tient dans un seul fichier. Pour la retirer, supprimez le fichier ; vos codes restent dans ~/.config/lambit2FA.

Fonctionne sur Ubuntu 22.04 et plus récent, Debian 12 et plus récent, Linux Mint 21 et plus récent, Pop!_OS 22.04 et plus récent, Fedora 38 et plus récent. Les autres distributions ne sont pas testées. Si le fichier ne s'ouvre pas, installez libfuse2 : sudo apt install libfuse2 (sur Ubuntu 24.04 : libfuse2t64).

Au premier lancement, le système peut demander le mot de passe du trousseau « login ». C'est le système qui demande, pas l'application : l'application range sa clé dans le trousseau du système. Saisissez le mot de passe du trousseau ou appuyez sur Annuler — la clé sera alors gardée dans un fichier lié à cet ordinateur et à votre utilisateur.

La lecture d'un code QR à l'écran sous Wayland nécessite un outil de capture (gnome-screenshot, spectacle ou grim). Sinon, faites vous-même une capture et ouvrez-la dans l'application comme image.

Vérifier le téléchargement : sha256sum lambit2FA-1.1-linux-x86_64.AppImage — le résultat doit correspondre au fichier .sha256 à côté.
