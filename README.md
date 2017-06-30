# vis.js on RoR

[![Gem Version](https://badge.fury.io/rb/vis-gem.svg)](https://badge.fury.io/rb/vis-gem)
[![Build Status](https://travis-ci.org/sniperwolf/vis-gem.svg?release=4.20.0.1)](https://travis-ci.org/sniperwolf/vis-gem)


A dynamic, browser based visualization library. The library is designed to be easy to use, to handle large amounts of dynamic data, and to enable manipulation of and interaction with the data. The library consists of the components DataSet, Timeline, Network, Graph2d and Graph3d.

More info to [vis.js official website](http://visjs.org/).

This gem wrap vis.js dependencies to assets pipeline in Rails (`=> 3.1`) project.

Thanks to [luciuschoi](https://github.com/luciuschoi/visjs-rails/) for the original idea.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'vis-gem'
```

And then execute:

```bash
$ bundle
```

Or install it yourself as:

```bash
$ gem install vis-gem
```

## Usage

1. Add this to `application.js` (`assets/javascripts/application.js`):

```ruby
//= require ...
//= require vis
//= require ...
```

2. Add this to `application.scss` (`assets/stylesheets/application.scss`):

```css
...
@import "vis";
...
```

3. And this to `config/initializers/assets.rb` (for assets):

```ruby
Rails.application.config.assets.precompile += %w( network/* )
```

See [original vis.js documentation](http://visjs.org/) for properties and methods.

## Changelog

- v4.2.0 : First Release;

## Contributing

See [Contributing](CONTRIBUTING.md) doc.

## License

(C) Fabrizio Fallico 2017, released under the [MIT license](LICENSE.md).
