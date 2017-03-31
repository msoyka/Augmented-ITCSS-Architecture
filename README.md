# Augment ITCSS
This is an augmented css folder structure that originates from the Inverted Triangle CSS architecture orginally created to assist in the building of easily scalable code bases that lessens the amount of cognitive overhead.

##### Table of Contents

1. [Architecture Scopes](#architecture-scopes)
1. [Global Scope's Basic Overview](#global-scopes-basic-overview)
1. [Modules & Frameworks Scope's Basic Overview](#modules-frameworks-scopes-basic-overview)
1. [The Integration of BEM](#the-integration-of-bem)
1. [Resources](#resources)
1. [Core Contributors](#core-contributors)
1. [License](#license)


***


## Architecture Scopes
Within the Augmented-ITCSS Framework, there are different directories based upon the needs of that specific scope. Feel free to tweek it to best fit your project's needs.

* **Global Scope**
  * The "Global Scope" is heavily copied from the original idea of the [itcss](http://itcss.io/) created by [Harry Roberts](https://twitter.com/csswizardry).


* **Module Scope**
  * The "Module Scope" is a restructuring of the "Objects" and "Components" layers of the original itcss architecture. It adds a new directory named "modules" to the architecture. This was added to give each module its own itcss architecture, which increases the ability to manage and scale modules effortlessly.


* **Frameworks Scope**
  * Similarly the the "Module Scope", the "Frameworks Scope" was created for layout specific modules. This creates a separation of powers between the modules and their frameworks, which will allow the freedom to pair frameworks and modules at your heart's content.


_[Back to top](#table-of-contents)_


***


### Global Scope's ITCSS - Basic Overview:
Lets talk about the purpose of each layer within the itcss' Global Scope architecture.

* **SETTINGS**
  * The Settings layer does not contain any styles. It only houses variables and other configuration needs.
  * Examples: breakpoints, animations, colors, spacers, font-size, line height, etc.


* **GENERIC**
  * The Generic layer is houses very high-level, far reaching styles that are commonly used on every web project.
  * Example: Normalize.css, Box-sizing, Form Input Resets, Headings Reset, etc.


* **TOOLS**
  * Mixins and functions that are used to make it easy to apply commonly used code chunks and logic to the other elements.
  * Example: positions, text-sizes, media-queries, fonts, cursors, etc.


* **UTILITIES**
  * Classes that can be applied to html elements or used within tools and other modules / frameworks to help with DRY coding techniques
  * Utilities help seperate general global styles to increaases flexiblity and can be added and changed freely.
  * Examples: color, font, text-size, padding, align, background, etc.


* **ELEMENTS**
  * All style directly associated to the html selectors.
  * Example: h1...h6, p, blockquote, body, html, hr, ul, ol, li, etc.


* **BUILDING BLOCKS**
  * All modules that are the smallest building block pieces that
  * will be used to create modules and frameworks in the form of macros.
  * These are simliar to elements, but they are styles using classes, not the html element themselves.
  * Example: svgs, button, links, ux, inputs, responsive images, etc.


* **MODULES**
  * Modules are coding the main coding chunks of the project.
  * These utilize building blocks and custom styles and are placed within frameworks.
  * These pieces fit inside frameworks, but understanding the seperation can be subjective
  * Example: navigation, banner, hero-banner, etc.


* **FRAMEWORKS**
  * Frameworks are pices of code that wrap around modules to ensure they are correctly layed out on the browser window. Generally associated with custom grid.
  * These pieces fit inside frameworks, but understanding the seperation can be subjective
  * Example: main-header, main-footer, sidebar, line-break grid, lightbox grid, thirds grid, etc.


* **TRUMPS**
  * All styles that must always trump all other styles. Therefor, they all have the !important tag attached to them.


_[Back to top](#table-of-contents)_


***


### Modules & Frameworks Scope's ITCSS - Basic Overview:
Lets talk about the purpose of each layer within the itcss' "Modules" and "Frameworks" Scope's architecture.

All "Modules" and "Frameworks" Scope's could all have any of the options listed in the "Global Scope's" description above. However, there are a couple additions that are important to note. Note: These are just the ones that pertain to our projects. Feel free to tweak based of your projects needs.

* **OBJECTS**
  *   These are concerned with styling non-cosmetic design patterns, or 'objects'.


* **COMPONENTS**
  * The Components layer is where we begin to style recognisable pieces of UI.


* **ANIMATIONS**
  * Applying animations to elements


* **PROGRESSIVE ENHANCEMENTS**
  * Create smooth degradation when browser capabilities decrease.


_[Back to top](#table-of-contents)_


***


### The Integration of BEM
[BEM](http://getbem.com/) (Block Element Modifier) is a methodology, that helps you to achieve reusable components and code sharing in the front-end. BEM naming conventions are how Module's and Framework's ITCSS Objects and ITCSS Components are organized. Refer to example below for clearer understanding of the file structure.


```
frameworks
  simple-framework
    simple-framework-objects
      _simple-framework-objects.styles.sass
      simple-framework-objects-block.sass
      simple-framework-objects-element.sass
      simple-framework-objects-modifier.sass
    simple-framework-components
      _simple-framework-components.styles.sass
      simple-framework-components-block.sass
      simple-framework-components-element.sass
      simple-framework-components-modifier.sass
```

_[Back to top](#table-of-contents)_


***


### Resources
* [ITCSS](http://itcss.io/)
* [Harry Roberts](https://twitter.com/csswizardry)
* [BEM](http://getbem.com/)

_[Back to top](#table-of-contents)_


***


### Core Contributors
* [Matthew Soyka](https://github.com/m-soyka)

_[Back to top](#table-of-contents)_


***


## License

###### The MIT License

Copyright (c) 2017 MilesHerndon

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

_[Back to top](#table-of-contents)_
