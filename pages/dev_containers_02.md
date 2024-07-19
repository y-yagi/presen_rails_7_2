# Development Containers is 何

* Dockerのコンテナで開発のすべて出来るようにしよう、という取り組み
  * コーディングだけでなく、テストの実行なども
* コンテナの構成は設定ファイル(`devcontainer.json`)に記載し、どの環境でも同じ内容でコンテナが動作するようになっている
* MicrosoftとGitHubが推進
  * VSCodeで使われている(た?)「VSCode Remote - Container」が前身
* 2022年に[仕様](https://github.com/devcontainers/spec)と、この仕様のための[CLI(Dev Container CLI)](https://github.com/devcontainers/cli)がOSSになり、VSCode以外でも使えるようになった
  * [IntelliJもサポートしてる](https://www.jetbrains.com/help/idea/connect-to-devcontainer.html)