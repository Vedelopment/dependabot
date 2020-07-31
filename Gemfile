# frozen_string_literal: true

source 'https://rubygems.org'

# Heroku uses the ruby version to configure your application's runtime.
ruby '2.5.5'

# the Community api
gem 'discourse_api', '~> 0.14.1'

# server/db
gem 'puma', '~> 3.10.0'
gem 'rack-canonical-host'
gem 'rack-utf8_sanitizer'
gem 'rails', '~> 5.2.4.3'
gem 'paranoia', '~> 2.0'
gem 'pg'
gem 'newrelic_rpm'
gem 'rack-host-redirect'
gem 'rack-timeout'

# logging
gem 'lograge'

# split testing
gem 'split', '~> 3.4.1', require: 'split/dashboard'

# assets
gem 'slim-rails'
gem 'sassc-rails'
gem 'bootstrap-sass'
gem 'bower-rails'
gem 'font-awesome-rails'
gem 'angular-rails-templates', '~> 1.0'
gem 'coffee-script-source', '~>1.8.0'
gem 'coffee-rails'
gem 'uglifier'
gem 'sprockets', '~> 3.0'
gem 'contentful'
gem 'contentful_model', '~> 1.0'
gem 'active_storage_validations'

# media
gem 'filepicker-rails'
gem 'paperclip'
gem 'paperclip-ffmpeg'
# aws-sdk 2.0 is not backwards compatible and will break
# paperclip. See: https://github.com/thoughtbot/paperclip/issues/1764
gem 'aws-sdk', '<2.0'
gem 'aws-sdk-s3', require: false
gem 'zencoder'
gem 'httparty'

# user agent / browser
gem 'browser'

# views
gem 'simple_form'
gem 'possessive'
gem 'valid_email'
gem 'draper'
gem 'jbuilder'
gem 'rabl'
gem 'eco'
gem 'oj'
gem 'redcarpet'
gem 'high_voltage'

# controllers
gem 'responders'

# misc
gem 'acts_as_list'
gem 'friendly_id', '~> 5.0.0'
gem 'iso8601'
# Tree hierarchy using PostreSQL's LTree extension.
gem 'ltree_hierarchy'
gem 'ar_after_transaction'
gem 'talkable'

# object manipulation
gem 'ice_nine'

# authorization/authentication
gem 'omniauth'
gem 'omniauth-facebook'
gem 'omniauth-google-oauth2'
gem 'bcrypt-ruby', '~>3.1.0'
gem 'omniauth-identity'
gem 'pundit', '~>1.1.0'

gem 'devise'
gem 'devise-two-factor'
gem 'devise_saml_authenticatable', '~> 1.5.0'
gem 'secure_headers'
gem 'doorkeeper', '~> 5.0', '>= 5.0.2'

gem 'rqrcode'

# Email
gem 'mandrill_mailer'
gem 'mandrill-api', require: 'mandrill'
gem 'gibbon'

# configuration
gem 'configatron'
gem 'rollout'

# money
gem 'stripe', '=3.5.1'
gem 'money'
gem 'paypal-sdk-rest', '1.6.0'
gem 'money-currencylayer-bank'
gem 'braintree', '2.99.0'
gem 'monetize', '~> 1.8'

# analytics
gem 'kmts', '~> 2.0.0'
gem 'analytics-ruby', '~> 2.0.0', require: 'segment/analytics'
gem 'simple_segment'

# logging
gem 'raygun4ruby'

# ActiveRecord
gem 'kaminari'
gem 'activerecord-import', '~> 0.17.0'

# TimeZone
gem 'geocoder'

# Async Jobs
gem 'resque', '~> 2.0'
gem 'resque-heroku-signals'
gem 'resque-scheduler'
gem 'resque-retry'

# Connection Pooling
gem 'connection_pool'

# Redis
gem 'redis'
gem 'redis-namespace'

# Admin
# need to use github version because rubygems version doesn't yet support rails 4
gem 'activeadmin'
# active-admin addons
gem 'activeadmin-sortable'
gem 'active_admin_datetimepicker'

# Content editing
gem 'x-editable-rails'

# hash helpers
gem 'hashie'

# zip libraries
gem 'rubyzip'

# track what's going on with our data
gem 'paper_trail', '~> 10.0.0'
gem 'paper_trail-association_tracking'

# JSONAPI https://jsonapi.org/
gem 'fast_jsonapi'

# assets
gem 'font_assets'
gem 'jquery_mobile_rails'

# caching
gem 'actionpack-action_caching'
gem 'dalli'
gem 'kgio'
gem 'memcachier'

# i18n
gem 'i18n-active_record', require: 'i18n/active_record'

# rate limiting
gem 'rack-attack'
gem 'ratelimit'

# SEO
gem 'sitemap_generator'

# parallel http request
gem 'typhoeus'

# Manage ENV variables
gem 'dotenv-rails'

# Detect URLs in display text
gem 'rails_autolink'

gem 'aasm'

gem 'slack-notifier'

gem 'jquery-rails', '~> 4.1'
gem 'jquery-ui-rails', '~> 5.0'

gem 'webpacker-react'

gem 'graphql', '~> 1.9'
gem 'graphql-batch'
source 'https://gems.graphql.pro/' do
  gem 'graphql-pro', '~> 1.10'
end

gem 'venice', '0.5.0', git: 'https://github.com/nomad/venice.git', ref: '1d416b1'

# Google
gem 'google-api-client', '~> 0.11'
# NOTE : Google Real Time Developer Notifications - v '0.23.2'
# can't update Pubsub, because omniauth-facebook faraday v <~ '0.11'
# Pubsub ~> '0.23.2' requires faraday v ~> '0.12'
gem 'google-cloud-pubsub'
gem 'google_drive'
gem 'migration_data'
gem 'algoliasearch-rails'
gem 'jwt', '>= 2.2.1'

gem 'memory_profiler'
gem 'system_cat'

# performance marketing
gem 'facebookbusiness', git: 'https://github.com/yankaindustries/facebook-ruby-business-sdk.git'
gem 'google-adwords-api'

group :test do
  gem 'approvals', require: 'approvals/rspec'
  gem 'rspec_junit_formatter', '0.2.2'
  gem 'stripe-ruby-mock', '= 2.5.0', require: 'stripe_mock'
  gem 'webmock'
  gem 'vcr'
  gem 'mock_redis'
  gem 'resque_spec'
  gem 'faker', '~> 1.9', '>= 1.9.1'
end

group :test, :development do
  gem 'railroady'
  gem 'awesome_print'
  gem 'rspec-rails'
  gem 'rspec-json_expectations'
  gem 'rspec-its'
  gem 'capybara'
  gem 'capybara-screenshot'
  gem 'poltergeist'
  gem 'factory_bot_rails'
  gem 'database_cleaner'
  gem 'fuubar'
  gem 'jasmine'
  gem 'jasmine-jquery-rails'
  gem 'timecop'
  gem 'shoulda-matchers', '4.0.0.rc1'
  gem 'simplecov'
  gem 'spring'
  gem 'pry'
  gem 'pry-remote'
  gem 'byebug'
  gem 'figaro'
  gem 'rspec-html-matchers'
  gem 'active_record_query_trace'
  gem 'parallel_tests'
  gem 'rails-controller-testing'
  gem 'rubocop', '~> 0.68.1', require: false
  gem 'rubocop-performance', '~> 1.2.0'
  gem 'rubocop-rspec', require: false
  gem 'spec_cat'
end

group :development do
  gem 'rack-livereload'
  gem 'spring-commands-rspec'
  gem 'foreman'
  gem 'rb-fsevent'
  gem 'growl'
  gem 'letter_opener'
  gem 'geoip'
  gem 'graphiql-rails'
  gem 'rails_best_practices', '~> 1.19.4'

  # code doctor
  gem 'bullet'
  gem 'meta_request'
end
