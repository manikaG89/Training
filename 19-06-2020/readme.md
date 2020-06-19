# What’s the difference between SCSS and Sass?

SCSS        |      Sass
------------------------------
Stands for Sassy CSS| Stands for Syntactically Awesome Style Sheets
----------------------------------------------------------------------
Similar to CSS (uses curly braces and semicolons)|Uses strict indentation (like Python)
----------------------------------------------------------------------------------------
Any valid CSS is valid SCSS | CSS code cannot be used as SASS
-----------------------------------------------------------------------------
.scss extension|   .sass extension
-----------------------------------------------------------------------

### Here’s an example of SCSS:
```
body {
  background-color:#000;
  color:#fff;
}
```

### Below is an example of Sass.
```
body
  background-color:#000;
  color:#fff;
  ```

 ## The structure of SCSS rules

 1. The structure of SCSS follows that of CSS. First, choose one or more elements using IDs, classes, or other CSS selectors. Then, add styles.

 2. In this example, we select the elements with button class and add some properties. This is valid as CSS code as well as SCSS code. It’s important to note that SCSS supports all CSS properties.

 ```
 .button {
  display:inline-block;
  font-size:14px;
  padding:4px 10px;
}
```

### Comments in SCSS

* Both // (single-line) and /* */ (multi-line) comments are allowed in SCSS.

```
// this is a single-line comment

/* this is a multi-line comment */
```

## The difference between SCSS and CSS variables

* SCSS variables are replaced with values when converted into CSS variables.
* These conversions take place before they are served to the browser, so browsers don’t even know there were variables in the first place, they just see the values.
* On the other hand, CSS variables are much more powerful.

## SCSS variable scope

* All variables defined in the top level are global.
* All variables defined in blocks (i.e., inside curly braces) are local.
* Blocks can access both local and global variables.

```
$my-global-variable: "I'm global";
div {
$my-local-variables: "I'm local";
}
```

## Changing the values of SCSS variables

* Changing values is done in the same way as declaring. When you change a variable, subsequent uses will have the new value while the previous uses remain unchanged.

```
$color: #fefefe;
.content {
  background-color: $color;
}

$color: #939393;
.footer {
  background-color: $color;
}
```
* Here, .content will have the background color #fefefe while .footer will have #939393. Global variables won’t change unless we add the !global modifier.

```
$color: #111;
.content {
  $color: #222; // this is a new local variable
  background-color: $color; # 222
}
.footer {
  $color: #333 !global; // changes the global variable  
}
```