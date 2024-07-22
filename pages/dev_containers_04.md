# Development Container Features

* Development Containersでは、Docker Imageを編集することなく、コンテナで使用するライブラリやCLIをインストールする事ができる。この機能を"Development Container Features"と呼んでいる
  * さっきの例だと、github-cliとmysql-cientをインストールするのに"Development Container Features"を使用している
  * 中身は普通にシェル

例：https://github.com/rails/devcontainer/blob/main/features/mysql-client/install.sh

```bash
#!/bin/sh
set -e

apt-get update -y && apt-get -y install --no-install-recommends default-mysql-client default-libmysqlclient-dev

rm -rf /var/lib/apt/lists/*
```

* [Available Dev Container Features](https://containers.dev/features)で使用出来るフィーチャーズの検索が出来る