# What is SASS?

* SASS (Syntactically Awesome Style Sheets) is a scripting language and CSS  preprocessor that compiles into CSS to make faster, easier, more elegant stylesheets.

* SASS adds new features and tools on top of basic CSS help organize stylesheets for large codebases in a maintainable, useful way. 


## What is a CSS preprocessor?

* SASS is a tool called a CSS preprocessor that can be used to code more maintainable CSS.

* A CSS preprocessor is essentially a scripting language that takes one type of data and converts it to another type.

* It extends the default capabilities of CSS by allowing us to generate CSS using the original language’s syntax, which can be compiled into CSS.

## SASS for CSS: Why you should be using a CSS preprocessor

* A CSS preprocessor has the potential to transform your productivity and frontend skills.

* After learning CSS, it’s the next natural step to advance your career. A CSS preprocessor speeds up development time and resolves many of the limitations of CSS.

# Advantages of using CSS Preprocessor

## They generate cleaner code due to nesting and variables.
* One huge advantage of SASS is that we can nest CSS selectors within selectors.

* This means that we only need to change the name of an element once.

* Similarly, with SASS, we can use variables. This allows you to store a value and reuse them throughout your files, simplifying your code overall!

## You keep your CSS code Dry (“Don’t repeat yourself”).
* Since you can now reuse code you’ve already written, you’re less likely to make mistakes, you stay more organized, and you save time by not repeating tasks.

* the code we write and test will continue to work no matter where we use it.

## They provide more flexibility.

* A CSS preprocessor resolves some of the rigid features of CSS.

* here are more things you can do spontaneously when you use a CSS preprocessor, such as conditionals or calculations. You can even modify colors on the fly so you don’t have to hard code them in CSS.

## They are more stable than CSS.

* A preprocessor adds a certain level of stability and maturity through features like mixins, nesting, inheritance, and more, which we will discuss shortly.

* the stability from a preprocessor makes it easier to handle large codebases.

## They make CSS code more organized. 

* Features like variables and functions mean you can shave off verbose CSS code, making it far more readable and organized. In the long run, organized code is easier to work with, share, and edit.

# Sass Features
### Variables
* Variables provide a way to store information or bundles of information that we can reuse throughout your stylesheet.

* For example, you could store color values or fonts that you can then reuse at any time in your CSS code.

* Variables save you tons of time rewriting that code, and it also prevents mistakes from cropping up along the way.

* Variables are particularly useful for large projects.
* Defining a variable is quite easy in SASS. You just need the $ symbol. Let’s look at an example where we define a color as a variable.

```
$color-primary: #ffff00; // Yellow
 
body {
  background-color: $color-primary;
}
```

### Nesting
* SASS adds nested syntax, which allows you to target DOM elements in a much cleaner way. 

* We no longer have to rewrite selectors multiple times.

```
.navbar {
  background-color: orangered;
  padding: 1rem;
}
.navbar ul {
  list-style: none;
}
.navbar li {
  text-align: center;
  margin: 1rem;
}
```

### Mixins
* Mixins allow you to group multiple lines of code together that you can reuse throughout your code.

* They are similar to functions in other programming languages.

* To create a mixin, you simply write your mixin and add it into the code using the @include directive wherever you want it. The mixin can be updated at any time.

```
@mixin transform {
  -webkit-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  transform: rotate(180deg);
}
```
```
@mixin transform {
  -webkit-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  transform: rotate(180deg);
}
```

### Partials and Importing
* SASS partials allow us to break up our files into smaller files.

* ou can create a partial file that only contains relevant code per section. This is useful if your SASS file is getting too large.

* The name of a partial begins with an _ underscore. It can then be imported at any time using the @import directive.

```
// In main.scss
@import 'header';

```

        