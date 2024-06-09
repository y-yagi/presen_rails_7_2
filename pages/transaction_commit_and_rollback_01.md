# Per transaction commit and rollback callbacks

* トランザクション毎にコミット/ロールバック時に実行するコールバックが登録出来るようになった

```ruby
Article.transaction do |transaction|
  article.update(published: true)

  transaction.after_commit do
    PublishNotificationMailer.with(article: article).deliver_later
  end
end
```

* 現在のトランザクションを取得する為のAPI(`ActiveRecord::Base.current_transaction`)も追加された

```ruby
Article.current_transaction.after_commit do
  PublishNotificationMailer.with(article: article).deliver_later
end
```
