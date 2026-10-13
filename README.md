lambit2FA for Linux — version 1.1

Two-factor login codes on your computer. No account and no internet needed. The codes are stored encrypted; the key lives in the system keyring (GNOME Keyring or KWallet) or, where there is none, in a file tied to this computer and your user.

For ordinary computers (Intel or AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

For ARM computers (Raspberry Pi 4/5, virtual machines on Apple Silicon, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

How to run: 1. Download the file. 2. Allow it to run: right-click → Properties → “Allow executing file as program”, or in a terminal: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Open it. Nothing gets installed — the app is one file. To remove it, delete the file; your codes stay in ~/.config/lambit2FA.

Works on Ubuntu 22.04 and newer, Debian 12 and newer, Linux Mint 21 and newer, Pop!_OS 22.04 and newer, Fedora 38 and newer. Other distributions are untested. If the file does not open, install libfuse2: sudo apt install libfuse2 (on Ubuntu 24.04: libfuse2t64).

On the first start the system may ask for the password of your “login” keyring. That is the system asking, not the app: the app puts its key into the system keyring. Enter the keyring password, or press Cancel — then the key is kept in a file tied to this computer and your user.

Reading a QR code from the screen on Wayland needs a screenshot tool (gnome-screenshot, spectacle or grim). Without one, take a screenshot yourself and open it in the app as a picture.

Check the download: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — the result must match the .sha256 file next to it.
