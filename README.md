体重をLineBOTに送ると前日比を返してくれるプログラム。
これを用いて毎朝の体重ツイートを行っている。

## 処理の流れ
- LineBOTからwebhookをcloudflare x honoに送信
- メッセージから数値を取得
- D1から最新の重量（=前日）を取り出す
- 前日比を計算
- D1に受け取った重量を保存
- Lineにメッセージを返す


