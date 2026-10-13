Linux 版 lambit2FA — バージョン 1.1

二要素認証のコードをあなたのコンピューターで。アカウントもインターネットも不要です。コードは暗号化して保存され、その鍵はシステムのキーリング（GNOME Keyring または KWallet）に、キーリングがない場合はこのコンピューターとあなたのユーザーに結び付いたファイルに保管されます。

一般的なコンピューター向け（Intel または AMD、x86_64）:
  lambit2FA-1.1-linux-x86_64.AppImage (38 MB)
  SHA-256: c982bbe2ab85bf8af552288a63b1adb8bcf5fb2a0e8bc75d0c6dfbb5195dcf6f

ARM コンピューター向け（Raspberry Pi 4/5、Apple Silicon 上の仮想マシン、aarch64）:
  lambit2FA-1.1-linux-aarch64.AppImage (36 MB)
  SHA-256: d97fab86f6f6904dad798f2fcda40e7921978d4a3fc5f94ffc75072f4c279c56

起動方法: 1. ファイルをダウンロードします。2. 実行を許可します: 右クリック → プロパティ → 「プログラムとして実行可能にする」、またはターミナルで chmod +x lambit2FA-1.1-linux-x86_64.AppImage。3. 開きます。何もインストールされません。アプリは 1 つのファイルです。削除するにはファイルを消してください。コードは ~/.config/lambit2FA に残ります。

Ubuntu 22.04 以降、Debian 12 以降、Linux Mint 21 以降、Pop!_OS 22.04 以降、Fedora 38 以降で動作します。その他のディストリビューションは未検証です。ファイルが開かない場合は libfuse2 を入れてください: sudo apt install libfuse2（Ubuntu 24.04 では libfuse2t64）。

初回起動時にシステムが「login」キーリングのパスワードを求めることがあります。尋ねているのはシステムであり、アプリではありません。アプリは自分の鍵をシステムのキーリングに保存します。キーリングのパスワードを入力するか、キャンセルを押してください。キャンセルすると、鍵はこのコンピューターとあなたのユーザーに結び付いたファイルに保管されます。

Wayland で画面から QR コードを読み取るにはスクリーンショットツール（gnome-screenshot、spectacle、grim）が必要です。ない場合は自分でスクリーンショットを撮り、アプリで画像として開いてください。

ダウンロードの確認: sha256sum lambit2FA-1.1-linux-x86_64.AppImage — 結果が隣の .sha256 ファイルと一致する必要があります。
