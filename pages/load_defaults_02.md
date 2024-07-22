# Default Values for Target Version 7.2

* `config.active_job.enqueue_after_transaction_commit: :default`
  * 本編中に説明した、`Prevent jobs from being scheduled within transactions`の挙動を指定するためのconfig
  * `:default`はアダプター次第
* `config.active_record.postgresql_adapter_decode_dates: true`
  * PostgreSQLAdapterでdate型のcolumnをSQLで直接取得した場合にDateとして扱うかどうかを指定
  * `ActiveRecord::Base.connection.select_value("select '2024-01-01'::date").class #=> Date`
* `config.active_record.validate_migration_timestamps: true`
  * マイグレーションファイルのタイムスタンププレフィックスが正しいフォーマットになっているかをチェックするかどうかを指定
  * タイムスタンプとして不正な値の場合、`ActiveRecord::UnknownMigrationVersionError`でエラーになる