## Sensu-Plugins-tempodb

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-tempodb.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-tempodb)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-tempodb.svg)](http://badge.fury.io/rb/sensu-plugins-tempodb)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-tempodb/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-tempodb)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-tempodb/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-tempodb)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-tempodb.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-tempodb)

## Functionality

## Files
 * bin/handler-tempodb

## Usage

```
{
    "tempodb": {
        "api_key": "your-api-key",
        "api_secret": "your-api-secret"
    }
}
```
## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-tempodb -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-tempodb`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-tempodb' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-tempodb' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
