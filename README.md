# 機能実装

- 試合の情報を取得
- サーバからレスポンス確認して準備確認
- 試合中にフィールドの状態取得
- agentの行動を送信
- TOKENが送信できているかの確認

# エンドポイント
- /matches 
    - GET
    - 試合開始前に事前に情報を取得する
- /matches/:matchID
    - GET
    - 試合の開始時間の取得
- /matches/:matchID/action
    - POST
    - Content-Type: application/json
    - Authorization: procon30_token
    - Agentの行動をpost
- /ping
    - headerにTOKENをつけた場合にアクセスできるかどうかの確認を行う