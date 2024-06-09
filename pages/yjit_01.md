# Enable YJIT by default if running Ruby 3.3+

* Ruby 3.3+の場合デフォルトでYJITが有効されるようになった
  * Ruby 3.3で追加された`RubyVM::YJIT.enable`を使用しているのでRuby 3.3+のみ
