# Default Progressive Web Application (PWA) files

* 新規アプリケーション作成時にProgressive Web Application (PWA) 用のファイルを生成するようになった
  * PWA自体の説明は[Progressive web apps \| MDN](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps)をご参照
* 生成されるのはServer Worker用のJSとマニフェストファイル
  * JSファイルにはPush通知用のコードが含まれている(コメントアウト)
  * ファイルは `app/views/pwa`に生成され、動的にrenderされるのでerbが書ける
* Rails 8.0でAction NotifierというPush通知用のコンポーネントを入れる予定がある
  * [Extract Action Notifier framework for push notifications](https://github.com/rails/rails/issues/50454)
