lambit2FA para Linux — versão 1.1

Códigos de início de sessão em dois passos no seu computador. Sem conta e sem Internet. Os códigos ficam cifrados; a chave está no porta-chaves do sistema (GNOME Keyring ou KWallet) ou, não havendo, num ficheiro ligado a este computador e ao seu utilizador.

Para computadores comuns (Intel ou AMD, x86_64):
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

Para computadores ARM (Raspberry Pi 4/5, máquinas virtuais em Apple Silicon, aarch64):
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

Como executar: 1. Transfira o ficheiro. 2. Permita a execução: botão direito → Propriedades → «Permitir executar o ficheiro como programa», ou no terminal: chmod +x lambit2FA-1.1-linux-x86_64.AppImage. 3. Abra-o. Nada é instalado — a app é um único ficheiro. Para remover, apague o ficheiro; os códigos ficam em ~/.config/lambit2FA.

Funciona em Ubuntu 22.04 ou mais recente, Debian 12 ou mais recente, Linux Mint 21 ou mais recente, Pop!_OS 22.04 ou mais recente, Fedora 38 ou mais recente. Outras distribuições não foram testadas. Se o ficheiro não abrir, instale libfuse2: sudo apt install libfuse2 (no Ubuntu 24.04: libfuse2t64).

No primeiro arranque o sistema pode pedir a palavra-passe do porta-chaves «login». É o sistema a perguntar, não a app: a app guarda a sua chave no porta-chaves do sistema. Escreva a palavra-passe do porta-chaves ou carregue em Cancelar — a chave fica então num ficheiro ligado a este computador e ao seu utilizador.

Ler um código QR do ecrã em Wayland precisa de uma ferramenta de captura (gnome-screenshot, spectacle ou grim). Sem ela, faça a captura você mesmo e abra-a na app como imagem.

Verificar a transferência: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — o resultado deve coincidir com o ficheiro .sha256 ao lado.
