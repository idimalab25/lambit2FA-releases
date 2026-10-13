lambit2FA cho Linux — phiên bản 1.1

Mã đăng nhập hai yếu tố trên máy tính của bạn. Không cần tài khoản, không cần Internet. Mã được lưu mã hóa; khóa nằm trong chùm khóa hệ thống (GNOME Keyring hoặc KWallet), hoặc nếu không có thì trong một tệp gắn với máy này và người dùng của bạn.

Cho máy tính thông thường (Intel hoặc AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

Cho máy tính ARM (Raspberry Pi 4/5, máy ảo trên Apple Silicon, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

Cách chạy: 1. Tải tệp về. 2. Cho phép chạy: chuột phải → Thuộc tính → “Cho phép thực thi tệp như chương trình”, hoặc trong terminal: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Mở tệp. Không cài đặt gì cả — ứng dụng là một tệp duy nhất. Để gỡ, xóa tệp; mã của bạn vẫn ở ~/.config/lambit2FA.

Chạy trên Ubuntu 22.04 trở lên, Debian 12 trở lên, Linux Mint 21 trở lên, Pop!_OS 22.04 trở lên, Fedora 38 trở lên. Các bản phân phối khác chưa được thử. Nếu tệp không mở, hãy cài libfuse2: sudo apt install libfuse2 (trên Ubuntu 24.04: libfuse2t64).

Lần chạy đầu tiên, hệ thống có thể hỏi mật khẩu chùm khóa “login”. Đó là hệ thống hỏi, không phải ứng dụng: ứng dụng đặt khóa của mình vào chùm khóa hệ thống. Hãy nhập mật khẩu chùm khóa hoặc nhấn Hủy — khi đó khóa được giữ trong một tệp gắn với máy này và người dùng của bạn.

Đọc mã QR từ màn hình trên Wayland cần công cụ chụp màn hình (gnome-screenshot, spectacle hoặc grim). Nếu không có, hãy tự chụp màn hình rồi mở trong ứng dụng dưới dạng ảnh.

Kiểm tra tệp tải về: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — kết quả phải khớp với tệp .sha256 bên cạnh.
