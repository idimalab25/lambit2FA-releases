lambit2FA dla Linuksa — wersja 1.1

Kody logowania dwuskładnikowego na Twoim komputerze. Bez konta i bez internetu. Kody są przechowywane zaszyfrowane; klucz leży w systemowym pęku kluczy (GNOME Keyring lub KWallet), a gdzie go nie ma — w pliku powiązanym z tym komputerem i Twoim użytkownikiem.

Dla zwykłych komputerów (Intel lub AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

Dla komputerów ARM (Raspberry Pi 4/5, maszyny wirtualne na Apple Silicon, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

Jak uruchomić: 1. Pobierz plik. 2. Zezwól na uruchamianie: prawy przycisk → Właściwości → „Zezwolenie na wykonywanie pliku jako programu”, albo w terminalu: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Otwórz go. Nic się nie instaluje — program to jeden plik. Aby usunąć, skasuj plik; kody zostają w ~/.config/lambit2FA.

Działa na Ubuntu 22.04 i nowszych, Debianie 12 i nowszych, Linux Mint 21 i nowszych, Pop!_OS 22.04 i nowszych, Fedorze 38 i nowszych. Inne dystrybucje nie były sprawdzane. Jeśli plik się nie otwiera, zainstaluj libfuse2: sudo apt install libfuse2 (na Ubuntu 24.04: libfuse2t64).

Przy pierwszym uruchomieniu system może zapytać o hasło pęku kluczy „login”. Pyta system, nie program: program wkłada swój klucz do systemowego pęku kluczy. Wpisz hasło pęku albo naciśnij Anuluj — wtedy klucz będzie trzymany w pliku powiązanym z tym komputerem i Twoim użytkownikiem.

Odczyt kodu QR z ekranu na Waylandzie wymaga narzędzia do zrzutów ekranu (gnome-screenshot, spectacle lub grim). Bez niego zrób zrzut sam i otwórz go w programie jako obrazek.

Sprawdzenie pobranego pliku: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — wynik musi zgadzać się z plikiem .sha256 obok.
