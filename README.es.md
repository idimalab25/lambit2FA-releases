lambit2FA para Linux — versión 1.1

Códigos de inicio de sesión en dos pasos en su ordenador. Sin cuenta y sin Internet. Los códigos se guardan cifrados; la clave está en el llavero del sistema (GNOME Keyring o KWallet) o, si no hay, en un archivo ligado a este equipo y a su usuario.

Para ordenadores corrientes (Intel o AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

Para ordenadores ARM (Raspberry Pi 4/5, máquinas virtuales en Apple Silicon, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

Cómo ejecutar: 1. Descargue el archivo. 2. Permita su ejecución: clic derecho → Propiedades → «Permitir ejecutar el archivo como un programa», o en un terminal: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Ábralo. No se instala nada: la aplicación es un solo archivo. Para quitarla, borre el archivo; sus códigos quedan en ~/.config/lambit2FA.

Funciona en Ubuntu 22.04 y posteriores, Debian 12 y posteriores, Linux Mint 21 y posteriores, Pop!_OS 22.04 y posteriores, Fedora 38 y posteriores. Otras distribuciones no se han probado. Si el archivo no se abre, instale libfuse2: sudo apt install libfuse2 (en Ubuntu 24.04: libfuse2t64).

En el primer inicio el sistema puede pedir la contraseña del llavero «login». Lo pide el sistema, no la aplicación: la aplicación guarda su clave en el llavero del sistema. Escriba la contraseña del llavero o pulse Cancelar; entonces la clave se guardará en un archivo ligado a este equipo y a su usuario.

Leer un código QR desde la pantalla en Wayland requiere una herramienta de captura (gnome-screenshot, spectacle o grim). Si no la hay, haga la captura usted mismo y ábrala en la aplicación como imagen.

Comprobar la descarga: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — el resultado debe coincidir con el archivo .sha256 de al lado.
