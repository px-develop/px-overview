# px-overview
運用ルールや総合的なドキュメント管理



## 運用ルール

- リポジトリ

  - 命名ルール

    - 構文

      ```javascript
      systemName-[ clientName | division ]-[ appId | appName ]-[ description ]
      ```
      - systemNameーシステム名（kintone, awsなど）
      - clinetNameークライアント名の略称（mjr, nccなど）
      - divisionー部署名の略称（ap, boなど）
      - appId/appNameーアプリID、アプリ名などを略して記載
      - descriptionーその他補足（任意）

    - 全角禁止

    - ケバブケース*で記載する　　*-(ハイフン)で単語をつなぐ

  - Description

    - 作成時にリポジトリの概要を記載する（日本語可）

  - README.md

    - システム構成、スクリプト構成、大まかな制御フローなどソフトウェア申請準拠レベルの内容を記載する
    - 別途ドキュメントに記載する場合はリンクを貼る（ドキュメント管理は後述）

- 運用フロー

  - 作業時はブランチを切る。ブランチ名は作業内容が分かるように記載する

    　ex) test-IconButton-bugFix

  - 作業が終わったらレビューを経てmasterブランチにマージする



## ディレクトリ構造

- distー配布用ファイル
- srcーソースファイル
- docsードキュメント
- package.json, mafest.jsonなどconfigファイルは直下に配置する



## ドキュメント管理

- docsディレクトリ配下に格納する

