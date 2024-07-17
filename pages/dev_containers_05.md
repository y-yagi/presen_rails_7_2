# Development containers configuration for applications

* 普段お使いのエディターやIDEがDevelopment Containersをサポートしていれば、追加のパッケージなどをホストにインストールすることなう、すぐ開発環境が作成出来る
* [Getting Started with Dev Containers](https://edgeguides.rubyonrails.org/getting_started_with_devcontainer.html)というDevelopment Containersでの開発について説明したガイドも増えた
* 関連して、[rails-new](https://github.com/rails/rails-new)というCLI(Rust製)も作られ、ローカルにRubyを入れずに`rails new`が可能に
  * `rails-new myapp`で実行出来る
  * これにより、このCLIとDockerがインストールされていれば、事前準備なしですぐRailsアプリケーションの開発が可能に