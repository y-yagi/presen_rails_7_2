# Default Values for Target Version 7.2

* `config.load_defaults 7.2`したときに変更になるconfigについて

```
config.active_job.enqueue_after_transaction_commit: :default
config.active_record.postgresql_adapter_decode_dates: true
config.active_record.validate_migration_timestamps: true
config.active_storage.web_image_content_types: %w[image/png image/jpeg image/gif image/webp]
config.yjit: true
```