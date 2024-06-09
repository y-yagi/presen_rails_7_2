# Set a new default for the Puma thread count

* デフォルトのPumaのスレッド数を5から3に変更
* 遅いSQLや、3rd partyのAPIの実行などの遅い処理がアプリケーションで実行されてスレッドが専有される事を考慮して、5としていた
* ただ、Railsはそれらの遅い処理はバックグラウンドジョブで実行する事を考慮しており、アプリケーションサーバで実行される処理は高速(なはず)
* その場合、5は多すぎるのでは、という話がそもそもあった
  * スレッドが多いと、GVLの解放を待つのに時間を費やしてしまい、レイテンシに悪影響を与える影響がある為
* 色々検証した結果、3が一番バランスが良いのでは、という事で3になった
* ベンチマーク等については、 [Set a new default for the Puma thread count](https://github.com/rails/rails/issues/50450) を参照
