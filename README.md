## Demo

A GitHub-hosted demo can be found here:  
[View project page](http://erming.github.io/jquery-string_to_color/)

## Install

Manual install:  
  1. Download [jquery.string_to_color.js](https://raw.githubusercontent.com/erming/jquery-string_to_color/gh-pages/jquery.string_to_color.js)
  2. Include source: `<script src="jquery.string_to_color.js"></script>`

## Usage

```
/**
 * Generate hex color code from a string.
 *
 * @param {String} string
 * @return {String}
 */
$.string_to_color(string);

/**
 * Set one or more CSS properties for the set
 * of matched elements.
 *
 * @param {String|Array} property
 * @param {String} string
 */
$(selector).string_to_color(property, string);
```

#### Here's some examples:
```
// Generate hex color.
var c = $.string_to_color("foo");
alert(c); // #0073ad

// Change border and font color.
$(".foo").string_to_color(["border-color", "color"], "foo");

// Iterate all links and color them.
$("a").each(function() {
  $(this).string_to_color("color", $(this).text());
});
```

## Credits

This plugin is based on [string_to_color](https://github.com/brandoncorbin/string_to_color) by [Brandon Corbin](https://github.com/brandoncorbin).
