# slick\_map\_css-rails

A stylesheet for displaying site maps directly from HTML unordered list.
This library is built upon [SlickMapCSS](http://astuteo.com/slickmap) and adds convenient features such as:

* integration with the assets pipeline
* TODO : add colors customization

## Installation

Add it to your Gemfile:

`gem 'slick_map_css-rails'`

Run the following command to install it:

`bundle install`

In your CSS manifest `application.css` add:

`//= require slick_map_css-rails'`

## Usage

(adapted from the original ReadMe.txt)

1. Create an HTML unordered list of links wrapped inside a `<div class="sitemap">`. SlickMap was designed to style actual linked navigation, not simply lists, so make sure to include anchor tags. See the [adapted example file](https://github.com/ddidier/slick_map_css-rails/blob/master/doc/index.html) for the correct formatting.

2. Within your HTML file, the link to your home page should be at the top of the unordered list and have the class of `.home`. This is required to pull the home page link out above the rest of the site tree.

3. The SlickMap default is 4 columns. In order to change the number of columns, you simply need to change the class of the `primary` unordered list (`col4`, `col5`, etc.). SlickMap CSS will accomodate 1 to 10 columns, some much better than others.

  NOTE: Due to Internet Explorer's difficulty in rounding numbers, you may find the farthest right column drops down instead of appearing in line. If need be, you can resolve this issue by adjusting the CSS to use a slightly smaller percentage than what you really need, i.e. (pun intended) 24.9% instead of 25%.

## Requirements

Tested with Rails 3.2 but it should work with Rails 3.1, or anything that uses the asset pipeline.

## Contributing to slick_map_css-rails

* Check out the latest master to make sure the feature hasn't been implemented or the bug hasn't been fixed yet.
* Check out the issue tracker to make sure someone already hasn't requested it and/or contributed it.
* Fork the project.
* Start a feature/bugfix branch.
* Commit and push until you are happy with your contribution.
* Make sure to add tests for it. This is important so I don't break it in a future version unintentionally.
* Please try not to mess with the Rakefile, version, or history. If you want to have your own version, or is otherwise necessary, that is fine, but please isolate to its own commit so I can cherry-pick around it.

## Copyright

Copyright (c) 2012 David DIDIER. See LICENSE.txt for further details.

[Astuteo SlickMapCSS](http://astuteo.com/slickmap/)
