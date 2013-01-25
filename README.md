GRUNTEND
========

Boilerplate for frontend development using [HTML5 Boilerplate](http://html5boilerplate.com/), mobile first styles, [CoffeeScript](http://coffeescript.org/) and [LESS](http://lesscss.org/). Built using [Grunt](http://gruntjs.com/).


Getting Started
---------------

Install [Node.js](http://nodejs.org/)

Install grunt:

	npm install -g grunt

Install plugins:

	npm install grunt-contrib

Build the site:

	grunt

The built site can be found at dist/

Grunt can watch the project and compile LESS and coffeescript when you make changes to the files. Grunt is setup to _not_ minify files when watching them to aid debugging whilst in development.

	grunt watch

Project build settings are configured in the usual `grunt.js` file.


HTML5 Boilerplate diff
----------------------

- `main.css` is renamed -> `base.less`. Your base styles for all screen widths greater than 0px go in `base.less`
- `normalize.css` renamed -> `normalize.less` to allow it to be imported inline into the compiled stylesheet
- There are extra stylesheets in for different screen widths `320.less`, `768.less` and `960.less`. Styles for screen width of 320px and above go in `320.less`, Styles for screen width of 768px and above go in `768.less` etc. There is also a `main.less` and `ie.less` stylesheet. `main.less` imports your stylesheets wrapped in the relevant @media query blocks. `ie.less` does the same, but doesn't use media queries.
- `index.html` includes the concatinated and minified CSS stylesheet (which includes normalise.css). lt-ie8 gets the `ie.less` stylesheet instead
- `main.js` renamed -> `main.coffee`


Changelog
---------

### 0.1.0

- Updated to HTML5 Boilerplate v4.1.0

### 0.0.1

- Brand new
- Using HTML5 Boilerplate v4.0.3 