# vis.js on RoR

[![Gem Version](https://badge.fury.io/rb/vis-gem.svg)](https://badge.fury.io/rb/vis-gem)
[![Build Status](https://travis-ci.org/sniperwolf/vis-gem.svg?release=4.20.0.2)](https://travis-ci.org/sniperwolf/vis-gem)

A dynamic, browser based visualization library. The library is designed to be easy to use, to handle large amounts of dynamic data, and to enable manipulation of and interaction with the data. More info at [vis.js official website](http://visjs.org/).

This gem wrap vis.js dependencies to assets pipeline in Rails (`=> 3.1`) project.

[Actual](https://github.com/sniperwolf/vis-gem/releases/tag/4.20.0.2) **vis.js version** is `4.20.0` (released on 21 May 2017, see [release notes](https://github.com/almende/vis/releases/tag/v4.20.0)).

Thanks to [luciuschoi](https://github.com/luciuschoi/visjs-rails/) for the original idea.

## Installation

Add this line to `Gemfile`:

```ruby
gem 'vis-gem'
```

And then execute:

```bash
$ bundle
```

Or install it with:

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

- `v4.2.0.2`: First Release with **vis.js** `v4.20.0` (released on 21 May 2017, see [release notes](https://github.com/almende/vis/releases/tag/v4.20.0)).

## Contributing

See [Contributing](CONTRIBUTING.md) document.

## License

(C) Fabrizio Fallico 2017, released under the [MIT license](LICENSE.md).
