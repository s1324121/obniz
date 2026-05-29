<img width="368" height="190" alt="Screenshot 2026-05-29 101541" src="https://github.com/user-attachments/assets/415b99b1-16f4-4020-a93b-61d334de8db2" />
<br>🏠 おかえり通知システム (obniz × LINE)
M5 Atom（obniz）とLINEを連携させた、子供の帰宅通知システムです。ブラウザ上のボタンを押すだけで、保護者のLINEに「ただいま」のメッセージが届きます。

(※リポジトリ内に画像をアップロードし、ファイル名を合わせてください)

🌟 主な機能
obniz IDの動的接続: 画面上の入力フォームから、使用するobniz IDを自由に切り替え可能。

LINE通知機能: Google Apps Script (GAS) を経由して、特定のLINEアカウントへ即座に通知。

LED演出: 通知送信時に、obnizに接続されたLEDテープ（WS2812）がカラフルに点灯します。

🛠 システム構成
ハードウェア: M5 Atom (obniz OS書き込み済み)

フロントエンド: HTML / JavaScript (jQuery, obniz.js)

バックエンド: Google Apps Script (GAS)

外部API: LINE Messaging API

🚀 使い方
1. 準備するもの
obniz ID (M5 Atomなど)

LINE公式アカウントのアクセストークン

デプロイ済みのGAS URL

2. 接続と実行
ブラウザで index.html を開きます。

上部の入力ボックスに obniz ID (例: 1234-5678) を入力し、「接続」ボタンを押します。

「接続完了！ ✅」と表示されたら準備完了です。

真ん中の大きな 「ただいま！」ボタン をクリックすると、LINEへ通知が飛びます。

📄 コードのポイント
連打防止機能: 送信中はボタンが無効化され、LEDが光っている間（約3秒間）は二重送信を防ぎます。

デバッグ表示: 接続状態をリアルタイムで画面に表示するため、トラブルシューティングが容易です。


