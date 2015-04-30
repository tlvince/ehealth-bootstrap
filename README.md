# [eHealth Africa Bootstrap Theme](http://ehealthafrica.org)

This theme is based on Bootstrap 3.0 and is to be used across all applications

## Table of contents

- [Quick start](#quick-start)
- [Custom eHealth Elements and Attributes](#custom-ehealth-elements-and-attributes)

## Quick start

Four quick start options are available:

- Clone the repo: `git clone https://github.com/twbs/bootstrap.git`.

Read the [Getting started page](http://getbootstrap.com/getting-started/) for information on the framework contents, templates and examples, and more.

## Custom eHealth Elements and Attributes

### Arrows for Alerts

The eHealth theme includes three additional class types to add a small arrow to any side of an alert box, to help make clear what the alert refers to:

![](screenshots/alert-arrow.png)

These are bootstrap style, so they require three classes to work:

  - `.arrow` for the base styles
  - `.arrow-dir-XX` for the direction of the arrow (`up`, `rt`, `dn` or `lt`)
  - `.arrow-pos-X` for the position along the respective edge (`t`, `r`, `b`, `l` or `c`), meaning top, right, bottom, left or center (avoid pointless combinations, such as `b` with `up` or `dn`)

The arrow automatically takes on the colour of the alert box.

So the red alert box with an arrow pointing up in the center (from the image above) is:

````
    <div class="alert alert-danger arrow arrow-dir-up arrow-pos-c"></div>
````

### Responsive helper classes for floating elements

Sometimes it is helpful to only pull an element on certain screen sizes. The
following helper classes allow to do exactly that:

  - `.pull-right-xs` and `.pull-left-xs`
  - `.pull-right-sm` and `.pull-left-sm`
  - `.pull-right-md` and `.pull-left-md`
  - `.pull-right-lg` and `.pull-left-lg`

In order to have an element be pulled right or left on multiple screen sizes
there are additional utility classes defined as follows:

  - `.pull-*-sm-min` and `.pull-*-sm-max`
  - `.pull-*-md-min` and `.pull-*-md-max`

So `.pull-right-sm-min` is basically a shortcut for not having to apply all of
`.pull-right-sm`, `.pull-right-md`, and `.pull-right-lg` together on the same
element.


## Documentation

Bootstrap's documentation, included in this repo in the root directory, is built with [Jekyll](http://jekyllrb.com) and publicly hosted on GitHub Pages at <http://getbootstrap.com>. The docs may also be run locally.

### Running Theme Locally

1. If necessary, [install Jekyll](http://jekyllrb.com/docs/installation) (requires v2.5.x).
  - **Windows users:** Read [this unofficial guide](http://jekyll-windows.juthilo.com/) to get Jekyll up and running without problems.
2. Install the Ruby-based syntax highlighter, [Rouge](https://github.com/jneen/rouge), with `gem install rouge`.
3. From the root `/bootstrap` directory, run `jekyll serve` in the command line.
4. Open <http://localhost:9001> in your browser, and voilà.

Learn more about using Jekyll by reading its [documentation](http://jekyllrb.com/docs/home/).

### Documentation for previous releases


[Previous releases](https://github.com/twbs/bootstrap/releases) and their documentation are also available for download.


## Contributing

Please read through our [contributing guidelines](https://github.com/twbs/bootstrap/blob/master/CONTRIBUTING.md). Included are directions for opening issues, coding standards, and notes on development.

Moreover, if your pull request contains JavaScript patches or features, you must include relevant unit tests. All HTML and CSS should conform to the [Code Guide](https://github.com/mdo/code-guide), maintained by [Mark Otto](https://github.com/mdo).

Editor preferences are available in the [editor config](https://github.com/twbs/bootstrap/blob/master/.editorconfig) for easy use in common text editors. Read more and download plugins at <http://editorconfig.org>.


## Versioning

For transparency into our release cycle and in striving to maintain backward compatibility, Bootstrap is maintained under [the Semantic Versioning guidelines](http://semver.org/). Sometimes we screw up, but we'll adhere to those rules whenever possible.



## Creators

**Brennan Novak**

- <https://brennannovak.com>
- <https://github.com/bnvk>


## Copyright and license

Code and documentation copyright 2014-15 eHealth Africa. Code released under [the MIT license](LICENSE). Docs released under [Creative Commons](docs/LICENSE).
