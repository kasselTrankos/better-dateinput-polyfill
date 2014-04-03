# better-dateinput-polyfill [![Build Status][travis-image]][travis-url] [![Coverage Status][coveralls-image]][coveralls-url]
> `input[type=date]` polyfill for [better-dom](https://github.com/chemerisuk/better-dom)

[VIEW DEMO](http://chemerisuk.github.io/better-dateinput-polyfill/)

## Features
* does nothing on mobile browsers and normalizes the widget for desktop browsers
* [live extension](https://github.com/chemerisuk/better-dom/wiki/Live-extensions) - works for current and future content
* supports US variant of date (just use `lang="en-US"` on `<html>`)
* calendar suppors navigation via keyboard
* allows to set value programmatically, but the string should be in ISO (yyyy-MM-dd) format
* fully customizable via css classes
* restores initial value on parent form reset

Installing
----------
Use [bower](http://bower.io/) to download this extension with all required dependencies.

    bower install better-dateinput-polyfill

This will clone the latest version of the __better-dateinput-polyfill__ into the `bower_components` directory at the root of your project.

Then append the following script on your page:

```html
<html>
<head>
    ...
    <link href="bower_components/better-dateinput-polyfill/dist/better-dateinput-polyfill.css" rel="stylesheet"/>
    <!--[if IE]>
        <link href="bower_components/better-dom/dist/better-dom-legacy.htc" rel="htc"/>
        <script src="bower_components/better-dom/dist/better-dom-legacy.js"></script>
    <![endif]-->
</head>
<body>
    ...
    <script src="bower_components/better-dom/dist/better-dom.js"></script>
    <script src="bower_components/better-dateinput-polyfill/dist/better-dateinput-polyfill.js"></script>
</body>
</html>
```

## Browser support
#### Desktop
* Chrome
* Safari 6.0+
* Firefox 16+
* Opera 12.10+
* IE8+

#### Mobile
* iOS Safari 6+
* Android 2.3+
* Chrome for Android

[travis-url]: http://travis-ci.org/chemerisuk/better-dateinput-polyfill
[travis-image]: https://api.travis-ci.org/chemerisuk/better-dateinput-polyfill.png?branch=master

[coveralls-url]: https://coveralls.io/r/chemerisuk/better-dateinput-polyfill
[coveralls-image]: https://coveralls.io/repos/chemerisuk/better-dateinput-polyfill/badge.png?branch=master
