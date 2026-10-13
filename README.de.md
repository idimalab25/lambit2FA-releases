lambit2FA für Linux — Version 1.1

Codes für die Zwei-Faktor-Anmeldung auf Ihrem Computer. Kein Konto, kein Internet nötig. Die Codes sind verschlüsselt gespeichert; der Schlüssel liegt im Schlüsselbund des Systems (GNOME Keyring oder KWallet) oder, wo es keinen gibt, in einer Datei, die an diesen Computer und Ihren Benutzer gebunden ist.

Für gewöhnliche Computer (Intel oder AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

Für ARM-Computer (Raspberry Pi 4/5, virtuelle Maschinen auf Apple Silicon, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

So starten Sie: 1. Datei herunterladen. 2. Ausführen erlauben: Rechtsklick → Eigenschaften → „Datei als Programm ausführen“, oder im Terminal: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Öffnen. Es wird nichts installiert — die App ist eine einzige Datei. Zum Entfernen die Datei löschen; die Codes bleiben in ~/.config/lambit2FA.

Läuft auf Ubuntu 22.04 und neuer, Debian 12 und neuer, Linux Mint 21 und neuer, Pop!_OS 22.04 und neuer, Fedora 38 und neuer. Andere Distributionen sind ungetestet. Öffnet sich die Datei nicht, installieren Sie libfuse2: sudo apt install libfuse2 (auf Ubuntu 24.04: libfuse2t64).

Beim ersten Start kann das System nach dem Passwort des Schlüsselbunds „login“ fragen. Das fragt das System, nicht die App: Die App legt ihren Schlüssel im Schlüsselbund des Systems ab. Geben Sie das Schlüsselbund-Passwort ein oder drücken Sie Abbrechen — dann liegt der Schlüssel in einer Datei, die an diesen Computer und Ihren Benutzer gebunden ist.

Das Lesen eines QR-Codes vom Bildschirm braucht unter Wayland ein Bildschirmfoto-Werkzeug (gnome-screenshot, spectacle oder grim). Ohne ein solches machen Sie selbst ein Bildschirmfoto und öffnen es in der App als Bild.

Download prüfen: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — das Ergebnis muss mit der .sha256-Datei daneben übereinstimmen.
