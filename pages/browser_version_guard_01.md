# Add browser version guard by default

* コントローラー/アクションへのアクセスをブラウザのバージョンを元に制限する[API](https://edgeapi.rubyonrails.org/classes/ActionController/AllowBrowser/ClassMethods.html#method-i-allow_browser)を追加

```ruby
class ApplicationController < ActionController::Base
  # webp images, web push, badges, import maps, CSS nesting + :hasをサポートしているブラウザ
  # (Safari 17.2+, Chrome 120+, Firefox 121+, Opera 106+)のみ許可
  allow_browser versions: :modern
end

class ApplicationController < ActionController::Base
  # ChromeとOperaは全てのバージョンを許可、IEは全て不許可、Safariは16.4+、Firefoxは121+のみ許可
  allow_browser versions: { safari: 16.4, firefox: 121, ie: false }
end

class MessagesController < ApplicationController
  # `show` actionでのみチェックを実施
  allow_browser versions: { opera: 104, chrome: 119 }, only: :show
end
```

* 不許可の場合、"406 Not Acceptable"が返る
  * エラー時に表示させるviewはデフォルトは`public/406-unsupported-browser.html`で、変更可能