# Setup jemalloc in default Dockerfile to optimize memory allocation

* 新規にアプリケーションを作成した際に生成されるDockerfileでjemallocのセットアップを行うよう変更
* なぜjemallocを使うのが良いかについてはオンラインに色々記事があるので、そちらをご参照さい
  * [Malloc Can Double Multi\-threaded Ruby Program Memory Usage](https://www.speedshop.co/2017/12/04/malloc-doubles-ruby-memory.html) とか
