# Development containers configuration for applications

* 新規にアプリケーションを作成した際に、[Development Containers](https://containers.dev/)用のファイルを生成するよう変更
* Redis、DBだけでなくHeadless Chromeなどもインストールされるようになっており、テスト等も含むローカルでの開発をすべてコンテナで実行出来るようになっている
* Railsではローカル(Docker及びDocker Composeを使用)で動く
* [Getting Started with Dev Containers](https://edgeguides.rubyonrails.org/getting_started_with_devcontainer.html)というDevelopment Containersでの開発について説明したガイドも増えた