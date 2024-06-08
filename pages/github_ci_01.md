# Add GitHub CI workflow by default to new applications

* 新規にアプリケーションを作成した際に、GitHub ActionsでCIを実行する為の設定ファイルが生成されるようになった
* CIでは、テスト、Lint(Rubocop)、セキュリティチェック(brakemanとimportmap-railsのaudit)が実行されるようになっている
