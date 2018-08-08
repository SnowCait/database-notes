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
