## Jasper2

[![Build Status](https://travis-ci.org/UMass-Makerspace/blog2.svg?branch=master)](https://travis-ci.org/umass-makerspace/blog2)
[![Ruby](https://img.shields.io/badge/ruby-2.5.1-blue.svg?style=flat)](http://travis-ci.org/umass-makerspace/blog2/)
[![Jekyll](https://img.shields.io/badge/jekyll-3.7.4-blue.svg?style=flat)](http://travis-ci.org/umass-makerspace/blog2)

This is a full-featured port of Ghost's default theme [Casper](https://github.com/tryghost/casper)
*v2.1.9* for [Jekyll](https://jekyllrb.com/) / [GitHub Pages](https://pages.github.com/).

## Features

* Out of the box support for multiple authors (via `_data/authors.yml`)
* Full author information including: picture, bio, website, twitter, facebook, etc.
* Tag description(s) and personalised covers (via `_data/tags.yml`)
* Related posts view at the bottom of each post
* All Ghost default pages: Author page(s), Tag page(s), About page(s), 404, etc.
* Pagination (infinite scrolling or standard pagination, i.e. posts across multiple pages)
* Atom Feeds by [Jekyll-feed](https://github.com/jekyll/jekyll-feed)
* Toggleable subscribe button (requires an external service)
* Code Syntax Highlight with [highlight.js](https://highlightjs.org/)
* Support for Google Analytics tracking
* Support for Disqus comments (not Ghost standard)

### Author Pages

In order to properly generate author pages you need to rename the field *author* in the
front matter of every post to match that of your each author's *username* as defined
in the *[\_data/authors.yml](_data/authors.yml)* file.
With the latest update, multiple author blogs are now supported out of the box.

## Copyright & License

Same licence as the one provided by Ghost's team. See Casper's theme [license](GHOST.txt).

Copyright (C) 2015-2018 - Released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
