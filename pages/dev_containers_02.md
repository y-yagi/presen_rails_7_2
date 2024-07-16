# Development Containers is 何

* 開発のすべてをDockerコンテナで出来るようにしよう、という取り組み
  * コーディングだけでなく、テストなども含む
* MicrosoftとGitHubが推進
* 開発環境をDockerコンテナとしてビルドし、ソースコードを管理・共有できるようにするための仕様
  * VSCodeで使われている(た?)「VSCode Remote - Container」が前身
* 2022年に仕様とこの仕様のためのCLI(Dev Container CLI)がOSSになり、VS Code以外でも使えるようになった
  * IntelliJもサポートしてる
  * [Dev Containers \| IntelliJ IDEA Documentation](https://www.jetbrains.com/help/idea/connect-to-devcontainer.html)