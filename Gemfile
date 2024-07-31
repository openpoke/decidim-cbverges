# frozen_string_literal: true

source "https://rubygems.org"

ruby RUBY_VERSION
DECIDIM_VERSION={ github: "decidim/decidim", branch: "release/0.28-stable" }

gem "decidim", DECIDIM_VERSION
gem "decidim-conferences", DECIDIM_VERSION
gem "decidim-templates", DECIDIM_VERSION
gem "decidim-decidim_awesome", github: "decidim-ice/decidim-module-decidim_awesome"
gem "decidim-term_customizer", github: "mainio/decidim-module-term_customizer"
gem "decidim-reporting_proposals", github: "openpoke/decidim-module-reporting_proposals"

gem "bootsnap", "~> 1.7"
gem "ffi", "~> 1.16.3"

gem "puma", ">= 6.3.1"
gem "deface", ">= 1.9"

group :development, :test do
  gem "byebug", "~> 11.0", platform: :mri
  gem "faker", "~> 3.2"

  gem "decidim-dev", DECIDIM_VERSION

  gem "brakeman", "~> 5.4"
end

group :development do
  gem "letter_opener_web"
  gem "listen"
  gem "spring"
  gem "spring-watcher-listen"
  gem "web-console"
end

group :production do
  gem 'aws-sdk-s3', require: false
  gem 'sidekiq'
  gem 'sidekiq-cron'
end
