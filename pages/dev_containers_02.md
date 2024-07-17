# Development Containers is 何

* 開発のすべてをDockerコンテナで出来るようにしよう、という取り組み
  * コーディングだけでなく、テストの実行なども
* MicrosoftとGitHubが推進
  * VSCodeで使われている(た?)「VSCode Remote - Container」が前身
* 2022年に[仕様](https://github.com/devcontainers/spec)と、この仕様のための[CLI(Dev Container CLI)](https://github.com/devcontainers/cli)がOSSになり、VSCode以外でも使えるようになった
  * IntelliJもサポートしてる
  * [Dev Containers \| IntelliJ IDEA Documentation](https://www.jetbrains.com/help/idea/connect-to-devcontainer.html)
* 必要なのはDockerと、Development Containersを管理するための設定ファイル(devcontainer.json)