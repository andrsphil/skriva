source 'https://rubygems.org'

# Ensure that gems from GitHub are pulled via HTTPS
git_source(:github) { |repo| "https://github.com/#{repo}.git" }


ruby '2.4.2'
gem 'rails', '~> 5.2.0'

# Infrastructure
gem 'pg'                                    # Active Record database
gem 'puma', '~> 3.11'                       # app server
gem 'bootsnap', '>= 1.1.0', require: false  # reduced boot time through caching

# Code processors
gem 'sassc-rails', '~> 2.0.0'               # stylesheet preprocessor
gem 'uglifier', '>= 1.3.0'                  # JavaScript uglifier
gem 'webpacker', '~> 3.5.5'                 # frontend code packer

# Libraries & assets
gem 'clearance', '~> 1.16.1'                # authentication framework
gem 'http_accept_language'                  # Fetch language info from requests
gem 'jbuilder', '~> 2.5'                    # JSON API builder
gem 'normalize-rails', '~> 4.1'             # CSS resets
gem 'turbolinks', '~> 5'                    # page fetching


# Additional gems for development and test environments
group :development, :test do
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw] # debugger console
end


# Additional gems for development environment
group :development do
  gem 'web-console', '>= 3.3.0'             # interactive console
  gem 'listen', '>= 3.0.5', '< 3.2'         # listen to file changes
  gem 'spring'                              # keep app running in background
  gem 'spring-watcher-listen', '~> 2.0.0'   # connect spring to 'listen' gem
  gem 'letter_opener'                       # open mails locally
  gem 'rubocop'                             # code linter
end


# Additional gems for test environment
group :test do
  gem 'capybara', '>= 2.15', '< 4.0'        # Capybara system testing
  gem 'selenium-webdriver'                  # Selenium driver
  gem 'chromedriver-helper'                 # Chrome system tests
end


# Zoneinfo files for Windows
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
