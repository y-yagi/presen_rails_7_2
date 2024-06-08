# Add omakase RuboCop rules by default

* [rails/rubocop-rails-omakase](https://github.com/rails/rubocop-rails-omakase) が誕生
* 新規にアプリケーションを作成すると、↑が使われるよう設定されるようになっている

```yml
# Omakase Ruby styling for Rails
inherit_gem: { rubocop-rails-omakase: rubocop.yml }

# Overwrite or add rules to create your own house style
#
# # Use `[a, [b, c]]` not `[ a, [ b, c ] ]`
# Layout/SpaceInsideArrayLiteralBrackets:
#   Enabled: false
```

* 設定されるCopについては https://github.com/rails/rubocop-rails-omakase/blob/main/rubocop.yml をみてね
