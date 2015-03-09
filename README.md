# rbenv

This cookbook gives you and easy way to install rbenv for a single user

## Supported Platforms

Tested on ubuntu Trusty platforms.

## Attributes

## Usage

```ruby
include_recipe 'rbenv'

rbenv_source 'install rbenv for user vagrant' do
  user 'vagrant'
end

rbenv_install 'rbenv install ruby 2.2.1 for user vagrant' do
  user 'vagrant'
  ruby_version '2.2.1'
end

rbenv_gem 'install bundler to ruby 2.2.1 installed with rbenv for user vagrant' do
  user 'vagrant'
  ruby_version '2.2.1'
  gem_name 'bundler'
end
```

## License and Authors

Author:: Álvaro Faúndez (alvaro@faundez.net)
