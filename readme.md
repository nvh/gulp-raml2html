# [gulp](http://gulpjs.com/)-raml2html [![Build Status](https://travis-ci.org/walling/gulp-raml2html.svg?branch=master)](https://travis-ci.org/walling/gulp-raml2html) [![NPM version](https://badge.fury.io/js/gulp-raml2html.png)](http://badge.fury.io/js/gulp-raml2html) [![Dependency Status](https://gemnasium.com/walling/gulp-raml2html.png)](https://gemnasium.com/walling/gulp-raml2html)

A simple RAML to HTML documentation generator.

*If you have any difficulties with the output of this plugin, please use the [raml2html tracker](https://github.com/kevinrenskers/raml2html/issues).*

Install via [npm](https://npmjs.org/package/gulp-raml2html):

```
npm install gulp-raml2html --save-dev
```

Note that this plugin wraps [raml2html](https://github.com/kevinrenskers/raml2html).

## Example

```js
var gulp = require('gulp');
var raml2html = require('gulp-raml2html');

gulp.task('apidoc', function() {
  return gulp.src('api.raml')
    .pipe(raml2html())
    .pipe(gulp.dest('build'));
});
```

## API

### supportJsonInput
Type: boolean
Default value: `false`

When set to `true` it also takes JSON files as input (generated by the RAML parser).

## License

The code for gulp-raml2html is licensed under the MIT license. See `license.txt` file for more info.
