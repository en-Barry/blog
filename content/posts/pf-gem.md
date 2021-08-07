---
title: "Gem選定と使用感【PF振り返り】"
date: 2021-08-06T21:33:19+09:00
tags: ["Gem", "Rails", "Ruby", "技術選定"]
categories: ["ポートフォリオ"]
draft: true
---

ここではPFに使用したGemの選定理由、使用感などを記していこうと思います
  
## 使用しているGem一覧

```Gemfile
ruby '2.6.6'

gem 'rails', '6.0.3.5'

# Assets
gem 'hanmoto'
gem 'sass-rails'
gem 'webpacker', '~> 4.0'

# Database
gem 'mysql2', '>= 0.4.4'
gem 'redis-rails'

# App server
gem 'puma', '~> 4.1'

# UI/UX
gem 'html2slim'
gem 'jbuilder', '~> 2.7'
gem 'rails-i18n', '>= 5.1.3'
gem 'slim-rails'
gem 'turbolinks', '~> 5'

# Authentication
gem 'sorcery'

# Form
gem 'simple_form'

# Seeds
gem 'faker'
gem 'seed-fu'

# Uploader
gem 'asset_sync'
gem 'carrierwave', '2.1.1'
gem 'fog-aws'

# Storage
gem 'mini_magick', '4.11.0'

# Model
gem 'enum_help'

# 外部API
gem 'rakuten_web_service'

# SEO/OGP対策
gem 'meta-tags'

# Search
gem 'ransack'

# Error notification
gem 'exception_notification'
gem 'slack-notifier'

group :development, :test do
  # Debugger
  gem 'better_errors'
  gem 'binding_of_caller'
  gem 'byebug', platforms: %i[mri mingw x64_mingw]
  gem 'pry'
  gem 'pry-byebug'
  gem 'pry-doc'
  gem 'pry-rails'

  # CLI
  gem 'spring'
  gem 'spring-commands-rspec'
  gem 'spring-watcher-listen', '~> 2.0.0'

  # Code analyze
  gem 'rails_best_practices'
  gem 'rubocop'
  gem 'rubocop-checkstyle_formatter'
  gem 'rubocop-rails'
  gem 'scss_lint'
  gem 'slim_lint'

  # Test
  gem 'factory_bot_rails', '~> 6.1.0'
  gem 'rspec-rails', '~> 4.0.1'
end

group :development do
  # Access an interactive console on exception pages or by calling 'console' anywhere in the code.
  gem 'foreman'
  gem 'listen', '~> 3.2'
  gem 'web-console', '>= 3.3.0'
end

group :test do
  gem 'capybara'
  gem 'webdrivers'
end

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: %i[mingw mswin x64_mingw jruby]
```

## Gemの概要と選定理由

