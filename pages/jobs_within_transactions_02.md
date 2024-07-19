# Prevent jobs from being scheduled within transactions

* トランザクションがコミットされる前にジョブがエンキューされると、ジョブ実行用のプロセスが、コミット前にジョブをピック＆実行してしまいエラーになる、という事よくあり、そのための対策として挙動が変更された
* トランザクションがロールバックした場合、自動でデキューされるようになっている
* 逆にいうと、元々はエンキュー時にエラーになったらロールバックされていたのが、ロールバックされなくなる
* この挙動はアプリケーション全体またはジョブ毎に変更可能
  * 挙動の変更方法の詳細は、[Rails Guide](https://edgeguides.rubyonrails.org/configuring.html#config-active-job-enqueue-after-transaction-commit)を参照ください
