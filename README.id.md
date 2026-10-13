lambit2FA untuk Linux — versi 1.1

Kode masuk dua langkah di komputer Anda. Tanpa akun dan tanpa internet. Kode disimpan terenkripsi; kuncinya berada di ring kunci sistem (GNOME Keyring atau KWallet) atau, jika tidak ada, di berkas yang terikat pada komputer ini dan pengguna Anda.

Untuk komputer biasa (Intel atau AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

Untuk komputer ARM (Raspberry Pi 4/5, mesin virtual di Apple Silicon, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

Cara menjalankan: 1. Unduh berkasnya. 2. Izinkan dijalankan: klik kanan → Properti → “Izinkan menjalankan berkas sebagai program”, atau di terminal: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Buka. Tidak ada yang dipasang — aplikasi ini satu berkas. Untuk menghapus, hapus berkasnya; kode tetap ada di ~/.config/lambit2FA.

Berjalan di Ubuntu 22.04 ke atas, Debian 12 ke atas, Linux Mint 21 ke atas, Pop!_OS 22.04 ke atas, Fedora 38 ke atas. Distribusi lain belum diuji. Jika berkas tidak terbuka, pasang libfuse2: sudo apt install libfuse2 (di Ubuntu 24.04: libfuse2t64).

Saat pertama dijalankan, sistem mungkin meminta kata sandi ring kunci “login”. Yang meminta adalah sistem, bukan aplikasi: aplikasi menyimpan kuncinya di ring kunci sistem. Masukkan kata sandi ring kunci atau tekan Batal — maka kunci disimpan di berkas yang terikat pada komputer ini dan pengguna Anda.

Membaca kode QR dari layar di Wayland memerlukan alat tangkapan layar (gnome-screenshot, spectacle, atau grim). Jika tidak ada, ambil tangkapan layar sendiri dan buka di aplikasi sebagai gambar.

Periksa unduhan: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — hasilnya harus cocok dengan berkas .sha256 di sebelahnya.
