# Development containers configuration for applications

* Redis、DBだけでなくHeadless Chromeなどもインストールされるようになっており、テストもコンテナで実行出来るようになっている
* ローカル(Docker及びDocker Composeを使用)で動作
* [Getting Started with Dev Containers](https://edgeguides.rubyonrails.org/getting_started_with_devcontainer.html)というDevelopment Containersでの開発について説明したガイドも増えた
* 使用しているコンテナのイメージとフィーチャーズは[rails/devcontainer](https://github.com/rails/devcontainer)にある
* 関連して、[rails-new](https://github.com/rails/rails-new)というCLI(Rust製)も作られ、ローカルにRubyを入れずに`rails new`が可能に
  * `rails-new myapp`で実行出来る