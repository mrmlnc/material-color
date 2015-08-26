Material Design Color
==============

The colour palette, based on [Google's Material Design](http://www.google.com/design/spec/style/color.html), for use in your project.

Support
--------------

Support for all popular css preprocessors: [Less](http://lesscss.org/), [Sass](http://sass-lang.com/) and [Stylus](http://learnboost.github.io/stylus/).

Installation
--------------

* Download the files you need from the this repository;
* Bower: `$ bower install material-color --save`;
* Git: `$ git clone git://github.com/mrmlnc/material-color.git`;

How to use
--------------

Just import the file, whitch includes variables colors in your project.

```Less
  // Less, Scss, Stylus
  @import "lib/material-color";
````

If you use Bower, the path would be:

````
  bower_components/material-color/..
````

**The build variable:**

`(@|$)clr-(color)-(range)`

  - **(@|$)** - Sign of the variable in the preprocessor.
  - **(color)** - Color.
  - **(range)** - 100, 300, 700, A100 and so on. The default value of 500.

**Example:**

````Less
  @import "lib/material-color";

  .example-1 {
    background-color: @clr-blue;
  }

  .example-2 {
    background-color: @clr-green-700;
  }
````

**Additional variables**

Additional variables for text based on [Material Design Typography](http://www.google.com/design/spec/style/typography.html).

````Text
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
````

**Mixin**

There are provided lists of variables for looping through the colors. In order to use this functionality you must import file and call mixin(s):

```
  @import "mixins/class-generator";

  // Less
  .material-color-class("red"); // another color or "all"
  .material-color-class("red", background-color); // another property or empty (default: color)

  // Scss
  @include material-color-class("red"); // another color or "all"
  @include material-color-class("red", background-color); // another property or empty (default: color)

  // Stylus
  material-color-class('red'); // another color or 'all'
  material-color-class('red', background-color); // another property or empty (default: color)
```

## Thanks

 - **Ali Amini** &lt;aliamini.af@gmail.com&gt; ([@AliAmini](https://github.com/AliAmini))
 - **Chris Pawlukiewicz** &lt;hi@paynoattn.com&gt; ([@paynoattn](https://github.com/paynoattn))
