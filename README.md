[![Build Status](https://travis-ci.org/thukim/force-destroy.svg?branch=master)](https://travis-ci.org/thukim/force-destroy) [![Code Climate](https://codeclimate.com/github/thukim/force-destroy/badges/gpa.svg)](https://codeclimate.com/github/thukim/force-destroy) [![Inline docs](http://inch-ci.org/github/remote-exec/command-designer.png)](http://www.rubydoc.info/github/thukim/force-destroy) [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://thukim.mit-license.org)

# Force::Destroy

A small gem that forces deleting an ActiveRecord instance/collection together with its/their associations

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'force-destroy'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install force-destroy

## Usage

This gem automatically adds in the 2 methods below:
  - `force_destroy!`: helps you to delete an ActiveRecord instance together with its associations even if the callbacks return false or throw abort
  - `force_destroy_all!`: similar to `force_destroy!`, but instead of deleting only an ActiveRecord instance, it deletes an ActiveRecord collection

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/thukim/force-destroy. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

