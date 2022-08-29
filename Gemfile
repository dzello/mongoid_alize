source 'https://rubygems.org'

rails_version = ENV['RAILS_VERSION'] || "7.0.3"
gem "rails", "~> #{rails_version}"

mongoid_version = ENV['MONGOID_VERSION'] || "8.0.2"
gem "mongoid", "~> #{mongoid_version}"

gem "mongoid-compatibility"

group :development, :test do
  gem 'rspec', '~> 2.99'
  gem 'rr', '1.2.1'

  unless ENV['CI']
    gem 'guard'
    gem 'guard-rspec'
    gem 'ruby_gntp'
    gem 'rb-fsevent'

    # irb goodies
    gem 'awesome_print'
    gem 'wirble'
  end
end

