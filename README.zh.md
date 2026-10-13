Linux 版 lambit2FA — 1.1 版

两步验证码就在您的电脑上。无需账号，无需联网。验证码加密保存；密钥保存在系统密钥环（GNOME Keyring 或 KWallet）中，没有密钥环时则保存在与这台电脑和您的用户绑定的文件中。

普通电脑（Intel 或 AMD，x86_64）：
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

ARM 电脑（Raspberry Pi 4/5、Apple Silicon 上的虚拟机，aarch64）：
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

运行方法：1. 下载文件。2. 允许运行：右键 → 属性 → “允许作为程序执行”，或在终端中执行 chmod +x lambit2FA-1.1-linux-x86_64.AppImage。3. 打开它。不安装任何东西——应用就是一个文件。要删除，直接删掉文件即可；验证码仍保存在 ~/.config/lambit2FA。

支持 Ubuntu 22.04 及更新、Debian 12 及更新、Linux Mint 21 及更新、Pop!_OS 22.04 及更新、Fedora 38 及更新。其他发行版未测试。如果文件打不开，请安装 libfuse2：sudo apt install libfuse2（Ubuntu 24.04 上为 libfuse2t64）。

首次启动时系统可能会要求输入“login”密钥环的密码。这是系统在询问，不是应用：应用会把自己的密钥放进系统密钥环。输入密钥环密码，或点击“取消”——那样密钥会保存在与这台电脑和您的用户绑定的文件中。

在 Wayland 下从屏幕读取二维码需要截图工具（gnome-screenshot、spectacle 或 grim）。没有的话，请自己截图，然后在应用中以图片方式打开。

校验下载：sha256sum lambit2FA-1.1-linux-x86_64.AppImage — 结果必须与旁边的 .sha256 文件一致。
