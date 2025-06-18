source "https://rubygems.org"
# Hello! This is where you manage which Jekyll version is used to run.
# When you want to use a different version, change it below, save the
# file and run `bundle install`. Run Jekyll with `bundle exec`, like so:
#
#     bundle exec jekyll serve
#
# This will help ensure the proper Jekyll version is running.
# Happy Jekylling!
#gem "jekyll", "~> 4.0.0"
# This is the default theme for new Jekyll sites. You may change this to anything you like.
gem "jekyll", "~> 4.3"
gem "minima", "~> 2.5"

# Fix for missing stdlibs in Ruby 3.4+
gem 'csv'
gem 'logger'
gem 'bigdecimal'

# Plugins
gem 'bibtex-ruby', '>= 6.0.0'
gem "jekyll-scholar", "~> 7.2"
gem "jekyll-sitemap"
gem "jekyll-feed"
gem "jekyll-katex"

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
	gem "tzinfo", "~> 1.2"
	gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :install_if => Gem.win_platform?