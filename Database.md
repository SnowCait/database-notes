# Database

## 規約
- カラム名の命名規則
  - `snake_case`, `camelCase` or `PascalCase`
- 時刻を扱うカラムのルールを決める
  - `datetime` or `timestamp`
  - `created` or `create` / `createdAt` or `createdTime`
- UTC で保存 - JST で保存しても良いが統一する
- 文字コード
- auto increment な `id` カラムを全テーブルに持つか
- `IF EXISTS` はなるべく使わない
  - 意図しない実行を検知するため
- `.sql` ファイルには `use スキーマ名` を記載しない
  - 異なるスキーマに対して実行する場合があるため
- `COMMENT` は更新がしづらいので使わない

## INDEX
- PK に含まれたカラムを減らす場合ユニークにならなくなるので一度 truncate する
  - データが入っているとエラーになるがデータが入っていないと通ってしまうので注意

## メンテナンス
- ゴミが残らないようにするためにチェックする仕組みを作る
  - 未使用テーブル
  - ゴミデータ

## テーブル設計
- INSERT しかしないテーブルはログと兼用できるが、なるべくログはログとして独立させる
- ログテーブルは DEFAULT を使わず実際のデータを INSERT する

## 負荷テスト
- [mysqlslap](https://dev.mysql.com/doc/refman/5.6/ja/mysqlslap.html) - read/write の性能を測る
  - [mysqlslapを使ってRDSのMySQLについて各クラスのパフォーマンス測定](https://dev.classmethod.jp/cloud/aws/amazon-rds-performance-test-by-mysqlslap/)

## 主キー (PK)
- [DB設計について考えてみた。ナチュラルキーとサロゲートキーはどちらが良いのか？ | 株式会社AMG Solution](https://amg-solution.jp/blog/8980)
