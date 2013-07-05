Chopstick
=========

Chopstick is a mobile-first responsive Design Framework, created and maintaned by [Wijs](http://wijs.be) in Ghent, Belgium.

## Install

Make sure you [install compass](http://compass-style.org/install). Optionally, you can use [CodeKit](http://incident57.com/codekit/).

## Use

Using Chopstick is easy and light-weight. We try to keep the code as modular as possible. Simply put, you can look at it this way:

    Shared Library + Settings = Theme

The default theme uses settings from the settings file + components from the shared library. You can remove the entire theme and just use some components from the shared library, as you see fit. We don’t like too much default generated code and neither should you.

### Folder Structure

The SCSS part of Chopstick consists of two main folders: `scss/shared` and `scss/theme` and two main files: `scss/_settings.scss` and `scss/screen.scss`.

The `scss/shared` folder contains all of the necessary mixins, includes, extends and other stuff to help you code quicker. Nothing in this folder is ever directly compiled to CSS. You need to reference components of Chopstick from within your theme’s SCSS code. 

The `scss/theme` folder will contain your theme. Everything in this folder will be compiled to CSS if you import it in `screen.scss`. We have prepared what we believe are some sensible defaults in the directory root and theme-specific modules in the `modules` folder, but feel free to delete anything in this folder you don’t like. Also remember to remove the import rules from the `screen.scss` file.

The `scss/_settings.scss` file contains all of the settings and variables you can use throughout your project. Again, we have prepared some sensible defaults to work with our framework, but feel free to add your own variables as you see fit.

The `scss/screen.scss` file will be compiled to `css/screen.css`. Everything you want to compile needs to be referenced in this file.

## Authors

Simon Coudeville: <simon.coudeville@wijs.be>  
[@simoncoudeville](http://twitter.com/simoncoudeville)

Xavier Bertels: <xavier.bertels@wijs.be>  
[@xavez](http://twitter.com/xavez)

## Credits

We owe a ton of credits to the following projects for inspiration:

* Boilerplate
* Foundation and Bootstrap
* Semantic Grid System
* SMACSS
