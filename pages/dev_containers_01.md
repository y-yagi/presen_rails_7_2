# Development containers configuration for applications

* 新規にアプリケーションを作成した際に、[Development Containers](https://containers.dev/)用のファイルを生成するようになった
* デフォルトでは無効(Rails 7.2では)。生成したい場合、`rails new`に`--devcontainer`オプションを指定する必要がある
* 既存のアプリケーションでファイルを生成したい場合、`devcontainer`コマンドが追加されているので、そちらで使用すれば良いようになっている

```bash
$ ./bin/rails devcontainer
Generating Dev Container with the following options:
app_name: test_app
database: mysql2
active_storage: false
redis: true
system_test: false
node: false
      create  .devcontainer
      create  .devcontainer/devcontainer.json
      create  .devcontainer/Dockerfile
      create  .devcontainer/compose.yaml
```