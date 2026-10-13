Linux için lambit2FA — sürüm 1.1

İki aşamalı giriş kodları bilgisayarınızda. Hesap ve internet gerekmez. Kodlar şifreli saklanır; anahtar sistem anahtarlığında (GNOME Keyring veya KWallet) durur, anahtarlık yoksa bu bilgisayara ve kullanıcınıza bağlı bir dosyada.

Sıradan bilgisayarlar için (Intel veya AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

ARM bilgisayarlar için (Raspberry Pi 4/5, Apple Silicon üzerinde sanal makineler, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

Nasıl çalıştırılır: 1. Dosyayı indirin. 2. Çalıştırmaya izin verin: sağ tık → Özellikler → “Dosyayı program olarak çalıştırmaya izin ver”, ya da terminalde: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Açın. Hiçbir şey kurulmaz — uygulama tek bir dosyadır. Kaldırmak için dosyayı silin; kodlarınız ~/.config/lambit2FA içinde kalır.

Ubuntu 22.04 ve üstü, Debian 12 ve üstü, Linux Mint 21 ve üstü, Pop!_OS 22.04 ve üstü, Fedora 38 ve üstünde çalışır. Diğer dağıtımlar denenmemiştir. Dosya açılmıyorsa libfuse2 kurun: sudo apt install libfuse2 (Ubuntu 24.04’te: libfuse2t64).

İlk açılışta sistem “login” anahtarlığının parolasını sorabilir. Soran sistemdir, uygulama değil: uygulama anahtarını sistem anahtarlığına koyar. Anahtarlık parolasını girin ya da İptal’e basın — o zaman anahtar bu bilgisayara ve kullanıcınıza bağlı bir dosyada tutulur.

Wayland’da ekrandan QR kod okumak için bir ekran görüntüsü aracı gerekir (gnome-screenshot, spectacle veya grim). Yoksa ekran görüntüsünü kendiniz alın ve uygulamada görsel olarak açın.

İndirmeyi doğrulama: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — sonuç yanındaki .sha256 dosyasıyla eşleşmeli.
