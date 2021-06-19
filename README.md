# home

## 実装内容
---

- 「開発環境・テスト環境のみ」にデバッグ用の gem を追加して、`bundle install`を実行

```
group :development, :test do
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]
  # 次の3つを追加
  gem 'pry-byebug'
  gem 'pry-rails'
  gem 'pry-doc'
end
```

## 補足
---

以下は事前に導入済みです。

- `rails g controller`コマンドで生成されるファイルの設定
　- `config/initializers/generators.rb`
- プルリクのテンプレートの設定
　- `.github/pull_request_template.md`
- RuboCop の導入
