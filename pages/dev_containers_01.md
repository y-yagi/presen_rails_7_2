# Development containers configuration for applications

* 新規にアプリケーションを作成した際に、[Development Containers](https://containers.dev/)用のファイルを生成するよう変更
* Redis、DBだけでなくHeadless Chromeなどの設定も入るので、テストもすべてコンテナで実行出来るようになっている
* [Getting Started with Dev Containers](https://edgeguides.rubyonrails.org/getting_started_with_devcontainer.html)というDevelopment Containersでの開発について説明したガイドも増えた
* [rails-new](https://github.com/rails/rails-new)というCLI(Rust製)も作られ、ローカルにRubyを入れずに新規アプリケーションの作成が可能に
  * `rails-new myapp`で実行出来る