# Development Containers is 何

**設定ファイルの例**

```json
{
  "name": "mysqlcontainer",
  "dockerComposeFile": "compose.yaml",
  "service": "rails-app",
  "workspaceFolder": "/workspaces/${localWorkspaceFolderBasename}",

  "features": {
    "ghcr.io/devcontainers/features/github-cli:1": {},
    "ghcr.io/rails/devcontainer/features/mysql-client": {}
  },

  "containerEnv": {
    "CAPYBARA_SERVER_PORT": "45678",
    "SELENIUM_HOST": "selenium",
    "REDIS_URL": "redis://redis:6379/1",
    "DB_HOST": "mysql"
  },

  "forwardPorts": [3000, 3306, 6379],
  "postCreateCommand": "bin/setup"
}
```