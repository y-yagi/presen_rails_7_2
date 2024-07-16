# Development Containers is 何

* コンテナはDockerを使用。Docker Composeも使用出来る。
* Docker Imageを編集することなく、追加で使用するライブラリやCLIをインストールする事ができる。この機能を"Development Container Features"と呼んでいる
  * さっきの例だと、元だと、github-cliとmysql-cientをインストールするのに"Development Container Features"を使用している

例：https://github.com/rails/devcontainer/blob/main/features/mysql-client/install.sh

```bash
#!/bin/sh
set -e

apt-get update -y && apt-get -y install --no-install-recommends default-mysql-client default-libmysqlclient-dev

rm -rf /var/lib/apt/lists/*
```
