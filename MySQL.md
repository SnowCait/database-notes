# MySQL

## 全般
- [ソシャゲエンジニアの自分が開発に必須だなと思った知識（MySQL編） - Qiita](https://qiita.com/west-hiroaki/items/ea6ee53765282a9c86cb)

## キーワード
- [ネクストキーロック](https://dev.mysql.com/doc/refman/5.6/ja/innodb-next-key-locking.html)

## MVCC
- [MySQLのMVCC](https://qiita.com/nkriskeeic/items/24b7714b749d38bba87b)

## パーティション
- [MySQL :: MySQL 5.6 リファレンスマニュアル :: 19.6.1 パーティショニングキー、主キー、および一意キー](https://dev.mysql.com/doc/refman/5.6/ja/partitioning-limitations-partitioning-keys-unique-keys.html)

## クライアント
- コマンド
- [MySQL :: MySQL Workbench](https://www.mysql.com/jp/products/workbench/)
- [A5:SQL Mk-2 - フリーの汎用SQL開発ツール/ER図ツール .. 松原正和](https://a5m2.mmatsubara.com/)

## Optimize
- [Amazon RDS for MySQL が予想以上のストレージを使用するときのディスクストレージを最適化](https://aws.amazon.com/jp/premiumsupport/knowledge-center/rds-mysql-storage-optimization/)

## INSERT
- [MySQLに大量のデータを入れるときに最適な方法は？](http://naoberry.com/tech/mysqldata/)
- [SQLで大量のテストデータ作成 - Qiita](https://qiita.com/cobot00/items/8d59e0734314a88d74c7)

## ALTER
- [ALTER TABLEにかかる実行時間を見積もりたい - tom__bo’s Blog](https://tombo2.hatenablog.com/entry/2019/07/28/222203)

## ランダム
- [MySQL :: MySQL 5.6 リファレンスマニュアル :: 12.6.2 数学関数](https://dev.mysql.com/doc/refman/5.6/ja/mathematical-functions.html#function_rand)
- [MySQLで簡単にランダムなテストデータを作成する方法 - Qiita](https://qiita.com/tayasu/items/c5ddfc481d6b7cd8866d)
```sql
SELECT FLOOR(1 + RAND() * 10);
SELECT CEIL(RAND() * 10);
```

## ページング
`FOUND_ROWS()` が便利そう。
- [MySQL :: MySQL 5.6 リファレンスマニュアル :: 12.14 情報関数](https://dev.mysql.com/doc/refman/5.6/ja/information-functions.html#function_found-rows)
- [SQL CALC FOUND ROWSを使う - dondari](https://www.dondari.com/SQL_CALC_FOUND_ROWS%E3%82%92%E4%BD%BF%E3%81%86)
