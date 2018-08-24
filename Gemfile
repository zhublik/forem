# frozen_string_literal: true

source 'https://rubygems.org'

# gem 'forem-theme-base', :git => "git://github.com/radar/forem-theme-base", :branch => "master"

gemspec

gem 'pry-nav'
gem 'pry-rails'
gem 'select2-rails', '~> 3.5.4'

platforms :jruby do
  gem 'activerecord-jdbc-adapter', require: false
end

group :test do
  platforms :ruby, :mingw do
    gem 'forem-redcarpet', github: 'quevita2018/forem-redcarpet'
    gem 'mysql2'
    gem 'pg'
    gem 'sqlite3'
  end

  platforms :jruby do
    gem 'activerecord-jdbcmysql-adapter', require: false
    gem 'activerecord-jdbcpostgresql-adapter', require: false
    gem 'activerecord-jdbcsqlite3-adapter', require: false
    gem 'forem-kramdown', github: 'phlipper/forem-kramdown', branch: 'master'
  end
end
