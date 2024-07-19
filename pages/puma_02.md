# Set a new default for the Puma thread count

* なお、プロセス数のデフォルトも使用可能なCPUコアの数になるよう修正されている
  * コンテナの場合cgroupの値を使用している
* 変更になったのはPumaのconfig(puma.rb)だけなので、Rails 7.2を待た無くても変更可能
* PumaとCRubyのconcurrencyとperformanceのついて説明した[guide](https://edgeguides.rubyonrails.org/tuning_performance_for_deployment.html)も追加されたので、合わせてどうぞ
