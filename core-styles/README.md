![NewSpring Core Styles](http://images.newspring.cc/site/logos/default.png)

# NewSpring Core Styles - v0.1

Newspring Core Styles is a [OOCSS](http://ianstormtaylor.com/oocss-plus-sass-is-the-best-way-to-css/)
library for all NewSpring Web projects.  It is a collection of mixins, objects, and intents to create
the base UI and rhythm for all of our projects.

It is a [SASS](http://sass-lang.com) library that is dependent on the
[inuit.css](https://github.com/csswizardry/inuit.css) framework. NewSpring Core expands on the
little-to-no design stance that inuit takes and applys base styling inline with the work
we do on all of our sites.

This library is built on a [BEM](http://bem.info/)-style naming convention and
honed based on [work done by Nicolas Gallagher](https://gist.github.com/1309546).

The core is built for our developers and designers to be able to focus on writing new features
and spend more time in markup and less time in sass. The OO approach in the library is important
to allow it to live on all the sites that we work on at once.

NewSpring Core Styles give us design decisions with the ability to expand per site and page. It will feature
common UI patterns, a strong mixin library, and support for IE 9+, firefox, chrome, and safari.

**Use NewSpring Core Styles if:**

* You work at NewSpring Web
* You want a strong library of mixins and objects to make your markup awesome
* You understand/appreciate the value of OO code and the need for scalability
  and reuse.
* You are a confident/competent developer comfortable with OOCSS and Sass, as
  well as familiarity with OO principles in general.
* You like bourbon

## Browser Support

NewSpring Core is a modern library for modern browsers. It takes inuit.css' browser support using
[normalize.css](http://necolas.github.com/normalize.css/) and global
`box-sizing:border-box;` (optional).

## Installation

**Requires Sass 3.2**

NewSpring Core Styles v0.1+ is designed to be even more advanced than previous versions of
your favourite CSS framework! The core library is intended to be used
as a submodule which means you can always get the latest updates without
ever having to touch a line of library code.  In fact, changing this code after the 1.0 launch should be
done with great caution and approval from the NewSpring Web Team.

## Getting started

The NewSpring Core Styles are already included in the NewSpring/NewSpring repo as a submodule next to inuit.css.
The code never needs to be touched and should be included after inuit.css in the master import of each project.

* Everything in `assets/_source/vendor/core-styles/` is library code which **should not** be edited.
  If you `cd` into here you should see that this submodule will initially be on
  `(no branch)`, this is because the submodule points at a specific commit and
  not a branch. You can treat this directory like any other Git project which
  means you can `$ git checkout master` to get your submodule on the most
  up-to-date stable version of the core. To grab any new changes simply run
  `$ git pull` on the `master` branch.
* `_vars.scss` contains any project variables you need, as well as any overrides
  you wish to make to the inuit.css or core library. It also houses feature switches to
  turn inuit.css’ and NewSpring Core's objects and abstractions on and off as you need them.
* All mixins are avaliable by default when included in a project.

## How NewSpring Core Styles works

NewSpring Core Styles works in ‘layers’, not dissimilar to [SMACSS](http://smacss.com/). The
principle of the core architecture is levels of extension; each layer of code
extends the layer below.

More to be written here as the library gets developed.

## Footprint

Out of the box, NewSpring Core Styles is not huge, however it is **imperative** that you
only ever deploy a minified version of your compiled stylesheet to your live
environment. This libray compiles stright to minified output by default in the deploy process
however, on local dev systems is compiles not minified so you can see what happens on compile.


## Documentation

The offical docs and style guide for NewSpring Core Styles can be found on the docs.newspring.io site.
They will continue to be updated as changes are made. However, on top of that documentation,
usage of the ojbects are outlined in the code. Everything is heavily commented with example HTML. If you
struggle with anything please talk to [Brian](mailto:brian.kalwat@newspring.cc),
[James](mailto:james.baxley@newspring.cc), [Joshua](joshua.blankenship@newspring.cc), or
[Jon](mailto:jon.horton@newspring.cc) and we will try help out and use your
feedback to improve the documentation.

It is strongly encouraged that you thoroughly read the source of inuit.css’
files, particularly `_core-styles.scss`.

## License

Copyright 2013 NewSpring Church

Licensed under the Apache License, Version 2.0.

---

**NewSpring Core Styles is the best SASS library out there, and it’s ready to help reach 100,000+**
