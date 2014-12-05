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

**Less:**

````Less
  @import "lib/material-color";
````

**Sass:**

````Sass
  @import "lib/material-color"
````

**Stylus:**

````Stylus
  @import "lib/material-color"
````

If you use Bower, the path would be:

````
  bower_components/material-color/..
````

**The build variable:**

`(@|$)(prefix)-clr-(color)-(range)`

  - **(@|$)** - Sign of the variable in the preprocessor.
  - **(prefix)** - The prefix variable. Namespace of your variables and variables of the library. (With `material-color-prefixed` and without `material-color`)
  - **(color)** - Color.
  - **(range)** - 100, 300, 700, A100 and so on. The default value of 500.

**Example:**

````Less
  @import "lib/material-color";

  .example-1 {
    background-color: @md-clr-blue;
  }

  .example-2 {
    background-color: @md-clr-green-700;
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
