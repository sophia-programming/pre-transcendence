# 課題：リアルタイムでオンライン対戦ができるPongゲーム

- ゲームの基本部分を完成させた後に、様々なモジュールを導入して、機能を拡張する必要がある
- Mandatory partを完成させるのが優先。その後、Modulesに入る。

## frontend
- Bootstrapは主にHTML、CSS、JavaScriptで構成されたフロントエンドフレームワーク
- ReactやVueなどのJavaScriptフレームワークとは異なり、Bootstrapはより軽量で、主にUIコンポーネントとレスポンシブデザインのためのツール
- Bootstrapを使用することで、JavaScriptの複雑な実装を減らし、UIの構築に集中できるらしい


## backend
- もし実装するならRuby。だが、moduleのとこで書き換えることもできる。
- Djangoになりそう
  - フォームを簡単に作成したり、フォームに入力されたデータを簡単に操作できるようにしてくれる、多機能なフレームワークがある
  - DjangoではMTVモデルという設計思想
    - M（モデル)...DBに関連する設定やテーブル名、そのフィールド名や機能、設定など。該当するファイルは models.py
    - T（テンプレート）...フロントエンドにて、データを表示する機能。 該当するファイルはtemplatesフォルダ直下のhtmlファイル
    - V（ビュー）...テンプレート（フロントエンド）にてデータをユーザーに表示するために、バックエンドでそのデータを選択したり、整形したりする機能。該当するファイルはviews.py
  - 学習の容易さ:Pythonは読みやすく、シンプルな構文を持っている
  - Djangoの学習リソースや参考資料が豊富に存在
  - 大規模なデータベース管理や高セキュリティが必要な場合、Djangoが適している
  - Djangoで書かれたアプリ　例）Youtube,　Dropbox,　Instagramなど


## Database
- backendと同様、もし使用するのであればDatabase moduleに従う必要がある。
- PostgreSQLを使用
  - PostgreSQLとSQLiteの違い
    https://bigdata-tools.com/sql-db/
  - 複数の端末からDBに操作を試みるようなシステムは「クライアントサーバー型」→　PostgreSQL, MySQLどちらか
  - そのソフトウェア内で完結するようなデータのやり取りをしたい場合は「SQLite」
  - ほとんどの場合はDBといえば「クライアントサーバー型」。