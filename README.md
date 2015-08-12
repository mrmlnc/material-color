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
If you want to print colors for use in HTML as classes, set `$print-colors` and `$$print-list` in the top of `material-color-prefixed.scss` file.
example:

SCSS: 
```SCSS
//===================== $print-colors =========================\\
//= @default: true
//= if you don't want to print selectors, change value to: false
//==============================================================\\
$print-colors: true; 

//===================== $print-list ========================\\
//= you can specify some color levels to print
//= @default: true -> prints all colors
//= @type: list -> prints specified levels 
//==========================================================\\
$print-list: 500 900; // prints $clr-*, $clr-*-500, $clr-*-900

```
Compiled to(CSS):
```CSS
.c-red-500 { color: #f44336; }
.bgc-red-500 { background-color: #f44336; }
.c-red { color: #f44336; }
.bgc-red { background-color: #f44336; }
.c-red-900 { color: #b71c1c; }
.bgc-red-900 { background-color: #b71c1c; }

.c-pink-500 { color: #e91e63; }
.bgc-pink-500 { background-color: #e91e63; }
.c-pink { color: #e91e63; }
.bgc-pink { background-color: #e91e63; }
.c-pink-900 { color: #880e4f; }
.bgc-pink-900 { background-color: #880e4f; }
/* and other colors */
```


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
