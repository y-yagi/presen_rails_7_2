# Prevent jobs from being scheduled within transactions

* Active Recordのトランザクション内で、Active Jobを使用してのジョブのエンキューが行われた場合に、コミット後にジョブのエンキューを自動で行うよう修正

```ruby
Topic.transaction do
  topic = Topic.create

  NewTopicNotificationJob.perform_later(topic)
end
```

* 上記の場合、Rails 7.1まではコミット前に`NewTopicNotificationJob`がエンキューされていたが、Rails 7.2ではコミット後にエンキューされるようになった
