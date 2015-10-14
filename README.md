Manatí Base Theme
=============

Base theme for Manatí's Drupal 7 sites.

## Features
TODO

## Usage
**1. Install npm modules**

``` sh
$ npm install
```

**2. Run grunt**
``` sh
$ grunt
```

**3. Edit sass and js files**
``` sh
$ vim sass/style.scss
```
``` sh
$ vim src-js/script.js
```

**4. Enjoy**


## Notes

#### Autoprefixer
Autoprefixer is ran via postcss, and is configured for the last 2 versions, edit `Gruntfile.js` to adjust to your needs

#### Grunt
Grunt has two modes, default mode `$ grunt` is for develpment and will do the following

* Sass output will be **nested**
* Watch with livereload will be active for all sass and javscript files
* Javascript will not be uglyfied and comments will be preserved
* TODO make sure this list is complete

For production we have `$ grunt prod`, and will do the following

* Sass output will be **compressed**
* Watch will not run, so grunt will exit as soon as it's finish
* Javascript will be uglified and compressed
* TODO make sure this list is complete

#### Javascript
The `src-js` folder has the script.js that will be uglified by grunt and placed in the `js\script.min.js`, the theme is configured to use this file and not the one in src-js.

The folder `js/vendor` can be used to place any 3rd party js files, grunt will not touch or modify anything in this folder.