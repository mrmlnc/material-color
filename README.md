# Material Design Color

> The colour palette, based on [Google's Material Design](http://www.google.com/design/spec/style/color.html), for use in your project.

## Installation

  * git: `git clone git://github.com/mrmlnc/material-color.git`;
  * bower: `bower install --save material-color`
  * npm: `npm install --save material-design-color`;

## Supported languages

Support for all popular css preprocessors:

  * [Less](http://lesscss.org/)
  * [Sass](http://sass-lang.com/)
  * [Stylus](http://learnboost.github.io/stylus/)

## How to use

Just import the file, whitch includes variables colors in your project.

```less
// Less, SCSS, Stylus
@import "lib/material-color";
```

**The build variable:**

`(@|$)clr-(color)-(range)`

  * **(@|$)** - Sign of the variable in the preprocessor.
  * **(color)** - Color.
  * **(range)** - 100, 300, 700, A100 and so on. The default value of 500.

**Example:**

```less
@import "lib/material-color";

.example-1 {
  background-color: @clr-blue;
}

.example-2 {
  background-color: @clr-green-700;
}
```

**Additional variables**

Additional variables for text based on [Material Design Typography](http://www.google.com/design/spec/style/typography.html).

```
// Typography
clr-ui-display-4
clr-ui-display-3
clr-ui-display-2
clr-ui-display-1
clr-ui-headline
clr-ui-title
clr-ui-subhead-1
clr-ui-body-2
clr-ui-body-1
clr-ui-caption
clr-ui-menu
clr-ui-button
```

**Mixin**

There are provided lists of variables for looping through the colors. In order to use this functionality you must import file and call mixin(s):

```less
@import "mixins/class-generator";

// Less
.material-color-class("red"); // another color or "all"
.material-color-class("red", background-color); // another property or empty (default: color)

// SCSS
@include material-color-class("red"); // another color or "all"
@include material-color-class("red", background-color); // another property or empty (default: color)

// Stylus
material-color-class('red'); // another color or 'all'
material-color-class('red', background-color); // another property or empty (default: color)
```

## Thanks

  * **Ali Amini** &lt;aliamini.af@gmail.com&gt; ([@AliAmini](https://github.com/AliAmini))
  * **Chris Pawlukiewicz** &lt;hi@paynoattn.com&gt; ([@paynoattn](https://github.com/paynoattn))

## Changelog

See the [Releases section of our GitHub project](https://github.com/mrmlnc/material-color/releases) for changelogs for each release version.

## License

This software is released under the terms of the MIT license.
