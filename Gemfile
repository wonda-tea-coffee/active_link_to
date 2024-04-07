source 'http://rubygems.org'

gemspec

if ENV['RAILS_VERSION'] == 'edge'
  gem 'rails', git: 'https://github.com/rails/rails.git'
  gem 'rackup'
elsif ENV['RAILS_VERSION']
  gem 'rails', "~> #{ENV['RAILS_VERSION']}.0"
  gem 'rackup' if ENV['RAILS_VERSION'] > '7.1'
else
  gem 'rails'
end

group :test do
  gem 'minitest'
  gem 'rake'
  gem 'rack-test'
  gem 'nokogiri'
end
