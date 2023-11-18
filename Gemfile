source "https://rubygems.org"

ruby "3.2.2"

# Bundle edge Rails instead: gem "rails", github: "rails/rails", branch: "main"
gem "rails", "~> 7.1.2"

# The original asset pipeline for Rails [https://github.com/rails/sprockets-rails]
gem "sprockets-rails"

# Use sqlite3 as the database for Active Record
gem "sqlite3", "~> 1.4"

# Use the Puma web server [https://github.com/puma/puma]
gem "puma", ">= 5.0"

# Use JavaScript with ESM import maps [https://github.com/rails/importmap-rails]
gem "importmap-rails"

# Hotwire's SPA-like page accelerator [https://turbo.hotwired.dev]
gem "turbo-rails"

# Hotwire's modest JavaScript framework [https://stimulus.hotwired.dev]
gem "stimulus-rails"

# Use Tailwind CSS [https://github.com/rails/tailwindcss-rails]
gem "tailwindcss-rails"

# Build JSON APIs with ease [https://github.com/rails/jbuilder]
gem "jbuilder"

# Use Redis adapter to run Action Cable in production
# gem "redis", ">= 4.0.1"

# Use Kredis to get higher-level data types in Redis [https://github.com/rails/kredis]
# gem "kredis"

# Use Active Model has_secure_password [https://guides.rubyonrails.org/active_model_basics.html#securepassword]
# gem "bcrypt", "~> 3.1.7"

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem "tzinfo-data", platforms: %i[ windows jruby ]

# Reduces boot times through caching; required in config/boot.rb
gem "bootsnap", require: false

# Use Active Storage variants [https://guides.rubyonrails.org/active_storage_overview.html#transforming-images]
# gem "image_processing", "~> 1.2"

group :development, :test do
  # See https://guides.rubyonrails.org/debugging_rails_applications.html#debugging-with-the-debug-gem
  gem "debug", platforms: %i[ mri windows ]

  # Test framework
  #
  # * Rspec : https://github.com/rspec/rspec-rails
  # * SimpleCov : https://github.com/simplecov-ruby/simplecov
  %w[rspec-core rspec-expectations rspec-mocks rspec-rails rspec-support].each do |lib|
    gem lib, git: "https://github.com/rspec/#{lib}.git", branch: 'main'
  end
  gem "simplecov", require: false

  # LSP
  #
  # * RubyLSP : https://github.com/Shopify/ruby-lsp
  # * ErbLint :
  #     * RubyGems : https://github.com/Shopify/erb-lint
  #     * VSCode : https://github.com/manuelpuyol/vscode-erb-linter
  gem "ruby-lsp", require: false
  gem "erb_lint", require: false
  # Linter
  #
  # * Rubocop : https://github.com/rubocop/rubocop
  #     * Extensions : https://docs.rubocop.org/rubocop/1.57/extensions.html#official-extensions
  #         * rubocop-performance
  #         * rubocop-rails
  #         * rubocop-rake
  #         * rubocop-rspec
  gem "rubocop", "~> 1.57.2", require: false
  gem "rubocop-performance", "~> 1.19.1", require: false
  gem "rubocop-rails", "~> 2.20.2", require: false # "~> 2.22.1" is not compatible with standard-rails
  gem "rubocop-rake", "~> 0.6.0", require: false
  gem "rubocop-rspec", "~> 2.25.0", require: false
  # Standard Ruby for default rules of Rubocop
  #
  # * standard : https://github.com/standardrb/standard
  # * standard-rails : https://github.com/standardrb/standard-rails
  gem "standard", "~> 1.32.0", require: false
  gem "standard-rails", "~> 0.2.0", require: false
end

group :development do
  # Use console on exceptions pages [https://github.com/rails/web-console]
  gem "web-console"

  # Add speed badges [https://github.com/MiniProfiler/rack-mini-profiler]
  # gem "rack-mini-profiler"

  # Speed up commands on slow machines / big apps [https://github.com/rails/spring]
  # gem "spring"
end
