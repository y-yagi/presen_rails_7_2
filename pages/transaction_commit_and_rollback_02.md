# Per transaction commit and rollback callbacks

* さらに、全ての実行中のトランザクションがコミットされた場合に実行される`ActiveRecord.after_all_transactions_commit`も追加された

```ruby
def publish_article(article)
  article.update(published: true)

  ActiveRecord.after_all_transactions_commit do
    PublishNotificationMailer.with(article: article).deliver_later
  end
end
```

* オープンしているトランザクションが1つの場合、`after_commit`と同等
