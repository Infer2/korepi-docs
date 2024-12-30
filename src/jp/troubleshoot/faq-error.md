---
title: インジェクターエラー
icon: info
category:
  - トラブルシュート
tag:
  - Start
author: Schvis
order: 2
---

## よくあるエラー

### korepiが消えてしまうのはなぜですか?

ウイルス対策ソフトが無効になっていることを確認し、新しいフォルダを作成して除外項目に追加します。

![](/assets/images/docs/202312/virus.png)

除外フォルダ内にkorepiを展開し、再度実行する。

---
### ステータス: ライセンスキーが無効です。

新しく [キーを取得する](../guide/getkey.md) 必要があります。`⁠🔐｜verification`, キーが手に入らなかったり、キーが使えなかったりした場合は、キーの有効期限が切れるまで待たなければなりません。

`スポンサーは、F:リセットキーを使用することができます。`

### [DLL インジェクション] プロセスがクラッシュ、終了コード 0xc000005

 `cmd` を管理者として開き、以下のコマンドを書く：

`sfc /scannow`

その後、エラーが見つかった場合は、コンピュータを再起動して確認する。再起動しても解決しなかったり、エラーが見つからなかった場合は、次のコマンドを書いてください：

`DISM.exe /Online /Cleanup-Image /RestoreHealth`

チェックを終えたら、コンピュータを再起動して確認します。

うまくいかない場合は、Windowsを再インストールしてください。

---
### ImGUI：DirectX11バックエンドが正常に初期化されました。

インストールしたテーマが原因でエラーが発生している場合は、 `themes` フォルダーを消してください。

---
### システムはMSVCP140.dllを検出しませんでした。

 [Microsoft Visual Studio C++](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#visual-studio-2015-2017-2019-and-2022)　を更新してください。

 [DirectX](https://www.microsoft.com/en-us/download/details.aspx?id=35)　を更新してください

---
### ファイルが破損しています！このプログラムは変更されており、感染している可能性があります。

![](/assets/images/docs/202312/virus2.png)

この場合、ウイルス対策ソフトを使用して完全スキャンを行い、ウイルスが見つかった場合はそれらを削除し、再起動してから再度スキャンを行ってみてください。それでもうまくいかない場合は、Windowsを再インストールするのがこの問題を解決する最も簡単な方法です。

---
### タイムアウトに達しました

![](/assets/images/docs/202312/error1.png)

ルーターを再起動します。

ウイルス対策ソフトが接続をブロックしている可能性があります。それがタスクマネージャーにないことを確認してください。

VPNを使用して再試行してください。

ファイアウォールに影響を与えるアプリケーションをすべてオフにする。何も効果がない場合は、ネットワークに何らかの問題がある可能性があります。

---
### DLLインジェクションに失敗しました

colorpicker をアンインストールし、colorpicker をもう一度ダウンロードします。

---
### Windows は指定されたデバイス、パス、またはファイルにアクセスできません

![](/assets/images/docs/202312/error2.png)

まず[こちらへ](https://support.microsoft.com/en-us/topic/-windows-cannot-access-the-specified-device-path-or-file-error-when-you-try-to-install-update-or-start-a-program-or-file-46361133-47ed-6967-c13e-e75d3cc29657) そしてその当行の手順に従ってください。

また、投稿の解決策が進んだ後、ウイルス対策ソフトウェアをダウンロードして、完全なシステムチェックを実行してください。

今後問題が解決しない場合は、管理者として cmd を開き、次のように書きます。 `sfc /scannow`

その後、エラーがあった場合は、コンピュータを再起動して確認してください。

再起動しても問題が解決しなかった場合、またはエラーが発生しなかった場合は、次のコマンドを記述します。

`DISM.exe /Online /Cleanup-Image /RestoreHealth`

確認が完了しましたら、コンピュータを再起動して再度確認してください。

動作しない場合は、Windowsを再インストールします。

---
### 署名チェックサムの失敗

![](/assets/images/docs/202312/checksum.png)

サーバーがダウンまたはシャットダウンしています。サーバーがオンラインになるまで待ってください。

---
### エラー5 ゲームプロセスの作成に失敗しました。

![](/assets/images/docs/202312/error3.png)

`cfg.ini` を消去してください。

---
### SSL 接続エラー

![](/assets/images/docs/202312/error4.png)

PCを再起動し、ルーターを再起動します。

うまくいかない場合はVPNを使ってみてください。

---
### ゲームのバージョンを検出できませんでした

インジェクターを更新し、手順に沿ってください [ここ](../start/download.md)

---
### ファイル ok

cfg.json を削除してください。ファイルに問題がある可能性があります。

---
### UserAssembly.dllが初期化されていません。2秒間待機してください。

この行の後にインジェクターがクラッシュした場合は、次の手順を試してください。

PCのウイルス対策ソフトをすべてオフにします。

問題が解決しない場合`sfc /scannow` 管理者として cmd でコマンドを使用してください。

チェック後にエラーが見つかり、Windowsが解決できない場合は、 `DISM.exe /Online /Cleanup-Image /RestoreHealth` コマンドを使用します。

確認後、コンピューターを再起動し、colorpickerをもう一度実行してみてください。

エラーが繰り返し発生する場合は、Windows を出荷時にリセットしてください。

---
### データが存在しないか、サーバーエラーです。

![](/assets/images/docs/202312/error.png)

ライセンスの一時停止を解除し、再度お試しください。

---
### 現在のタイムスタンプを確認できません。

![](/assets/images/docs/202402/timestamp.png)

ケース 1:
- VPNを使用中にこのエラーが発生する可能性があります。VPNを無効にして再度お試しください。

ケース 2:
- PCの時刻が自動同期設定になっているか確認してください。

::: info もしあなたがイラン出身なら、代わりにVPNを使う必要があるかもしれません。
:::

---
### Unable to open file to write public key:

- This error might happen if you got your game installed in other drive other than your main drive `C:/` , to solve it you can reinstall the game to the main drive and run Korepi again.

---
### Failed to get response from https://md5c...

- This error might happen if your conection is not stable or your conection to the website its blocked, please copy the link and check if you can access it. If you can't access the website, using a VPN might help.

---
### Received code is not 200 from https://md5c...

- This Error will appear if your key is paused, please head to `🔐｜verification` and click on `Unpause Key` and type `Yes` on the pop-up.