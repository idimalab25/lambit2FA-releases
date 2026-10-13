Linux용 lambit2FA — 버전 1.1

2단계 로그인 코드를 내 컴퓨터에서. 계정도 인터넷도 필요 없습니다. 코드는 암호화되어 저장되며, 키는 시스템 키링(GNOME Keyring 또는 KWallet)에, 키링이 없으면 이 컴퓨터와 사용자에게 묶인 파일에 보관됩니다.

일반 컴퓨터용(Intel 또는 AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

ARM 컴퓨터용(Raspberry Pi 4/5, Apple Silicon의 가상 머신, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

실행 방법: 1. 파일을 내려받습니다. 2. 실행을 허용합니다: 오른쪽 클릭 → 속성 → “프로그램으로 실행 허용”, 또는 터미널에서 chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. 엽니다. 아무것도 설치되지 않습니다. 앱은 파일 하나입니다. 제거하려면 파일을 지우세요. 코드는 ~/.config/lambit2FA에 남습니다.

Ubuntu 22.04 이상, Debian 12 이상, Linux Mint 21 이상, Pop!_OS 22.04 이상, Fedora 38 이상에서 동작합니다. 다른 배포판은 확인하지 않았습니다. 파일이 열리지 않으면 libfuse2를 설치하세요: sudo apt install libfuse2 (Ubuntu 24.04에서는 libfuse2t64).

처음 실행할 때 시스템이 “login” 키링의 암호를 물을 수 있습니다. 묻는 쪽은 시스템이지 앱이 아닙니다. 앱은 자신의 키를 시스템 키링에 넣습니다. 키링 암호를 입력하거나 취소를 누르세요. 취소하면 키는 이 컴퓨터와 사용자에게 묶인 파일에 보관됩니다.

Wayland에서 화면의 QR 코드를 읽으려면 스크린샷 도구(gnome-screenshot, spectacle, grim)가 필요합니다. 없으면 직접 스크린샷을 찍어 앱에서 이미지로 여세요.

내려받은 파일 확인: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — 결과가 옆의 .sha256 파일과 일치해야 합니다.
