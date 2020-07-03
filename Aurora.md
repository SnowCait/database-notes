# AWS Aurora

- [[Amazon Aurora]クエリキャッシュ検証：高速となった理由の考察｜ブログ｜TOPICS｜MySQL](http://scsk-db.jp/mysql/topics/2017/12/18-105526.html)
- [Amazon Aurora ストレージと信頼性 - Amazon Aurora](https://docs.aws.amazon.com/ja_jp/AmazonRDS/latest/AuroraUserGuide/Aurora.Overview.StorageReliability.html)
  - 「シャットダウン後に起動」「再起動」のときのみ有効
  - 「停止」した場合は無効
    - 他の手段でのウォームアップ方法はない
