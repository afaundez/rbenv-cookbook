# Rbenv

This cookbook gives you and easy and clean rbenv install for a single user.

## Supported Platforms

Tested on ubuntu trusty and centos 6.1.

## Attributes

## Usage

```ruby
include_recipe 'rbenv'

rbenv_source 'vagrant'

rbenv_install '2.2.1' do
  user 'vagrant'
end

rbenv_gem 'bundler' do
  user 'vagrant'
  ruby_version '2.2.1'
end

rbenv_install '1.8.7-p370' do
  user 'vagrant'
end

rbenv_gem 'bundler' do
  user 'vagrant'
  ruby_version '1.8.7-p370'
  rubygems_version '1.6.2'
  action :upgrade
end
```

## License and Authors

Author:: Álvaro Faúndez (alvaro@faundez.net)
