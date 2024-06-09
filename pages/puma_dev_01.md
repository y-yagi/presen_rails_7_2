# Suggest puma-dev configuration in bin/setup

* `bin/setup`に[Puma-dev](https://github.com/puma/puma-dev)のセットアップ用の処理を追加
  * コメントアウトされており、デフォルトでは実行されない
* 合わせて、`ActionDispatch::HostAuthorization`で`.test`ドメインからのアクセスを許容するよう修正(dev環境のみ)
  * Puma-devが`.test`ドメインを使用する為
