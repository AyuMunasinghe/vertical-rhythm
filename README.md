# Vertical Rhythm

> Create typographical vertical rhythm in your CSS. LESS, Stylus and SASS/SCSS versions included.

This should get you to your goal faster than starting from scratch. Please customize it to work with your own project.


**Example list styles**

`vertical-rhythm.scss` and `vertical-rhythm.styl`

```scss
.rhythm {
  h3 + ul.bullet-list,
  h3 + ul.numbered-list,
  h3 + ul.alpha-list,
  h3 + ol.numbered-list {
    margin-top: ($line-height-base / 2);
  }
}
```

`vertical-rhythm.sass`

```sass
.rhythm
  h3 + ul.bullet-list,
  h3 + ul.numbered-list,
  h3 + ul.alpha-list,
  h3 + ol.numbered-list
    margin-top: ($line-height-base / 2)
```

`vertical-rhythm.less`

```less
.rhythm {
  h3 + ul.bullet-list,
  h3 + ul.numbered-list,
  h3 + ul.alpha-list,
  h3 + ol.numbered-list {
    margin-top: (@line-height-base / 2);
  }
}
```

Designed to be mostly framework agnostic, although the baseline styles for normalizing are borrowed from Bootstrap. This means `vertical-rhythm.{less,styl,scss,css}` will make a good drop-in component for Bootstrap, _but it can also be used standalone for any project_.


## How does this work?
In **vertical-rhythm.{less,styl,scss,css}** you will find two sections:


#### I. Typography Base
If you use Bootstrap or Foundation, just get rid these base styles before you drop `vertical-rhythm.{less,styl,sass,css}` into your project. This section is not strictly necessary for creating vertical rhythm, but the styles here are a great starting point for any project.


#### II. Vertical Rhythm
The `.rhythm` styles are designed with sensible defaults that you should be able to use as is. Expect to use these styles as examples though, because every project is different and you will probably need to customize before you achieve vertical rhythm with the typography in your own project.



## Get Started
  * Install with [Bower](https://github.com/bower/bower), `bower install vertical-rhythm`
  * clone the repo, `git clone git://github.com/jonschlinkert/vertical-rhythm.git`
  * or [download the latest version](https://github.com/jonschlinkert/vertical-rhythm/zipball/master)


## Issues, Requests and Contributions
  * Have a suggestion, requests or correction? Please [create an issue](https://github.com/jonschlinkert/vertical-rhythm/issues).
  * Contributions and requests are very welcome.
  * Please comment the code in your requests so I can easily and quickly evaluate it.


## Author

**Jon Schlinkert**

+ [twitter.com/jonschlinkert](http://twitter.com/jonschlinkert)
+ [github.com/jonschlinkert](http://github.com/jonschlinkert)
+ [jonschlinkert.com](http://www.jonschlinkert.com)


## Credit & Attribution

> The baseline section in this vertical-rhythm component was originally based on `type.less` from the excellent [Bootstrap](http://twitter.github.com/bootstrap), by [Mark Otto](https://github.com/mdo) and [Jacob Thornton](https://github.com/fat).

