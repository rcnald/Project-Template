<h1 align="center">Project Template</h1>

[![en-US](https://img.shields.io/badge/language-en--US-green)](https://github.com/rcnald/Project-Template/README.md)
[![pt-BR](https://img.shields.io/badge/language-pt--BR-gray)](https://github.com/rcnald/Project-Template/README.pt-BR.md)

## ♾️ Requirements

- [Node.js](https://nodejs.org/en/download/)


## ⚗️ Techs

This project used the following technologies:

<p align="left">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <img src="https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=sass&logoColor=white">
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white">
</p>

## 👨‍💻 How to use

| command line  | what does                          | notes               |
|---------------|------------------------------------|---------------------|
| npm install   | install dependencies(node_modules) | execute first, once |
| npm start     | run live:server,sass & tailwind    | on production       |
| npm run build | run autoprefixer                   | project is done     |

**npm install** must be executed when you git clone(download) the file to generate de 'node_modules' folder, within all dependencies to run the technologies.

**npm start** it starts, sass, tailwindcs live-compiler & live-server on [localhost:3000](https://localhost:3000) port. The compiled files it's going to be on 'dist' folder (only write codes in 'src' folder).

**npm run build** when the project is done, it agains compile, just the dist/css file, its runs autoprefixer plugin that prevent cross-browser issues.

## 🤔 How do I code?

You may questioned yourself, what's those 'letter-{name}' things on HTML classes? It's called [Namespaces](https://csswizardry.com/2015/03/more-transparent-ui-code-with-namespaces/), it's function is inform the type of the element and where to find it just by seen it. I particular use these:
  - `o-` - object
  - `c-` - component
  - `l-` - layout
  - `u-` - utilities
  - `t-` - themes
  - `is-/has-` - states
  - `js-` - DOM elements

...Ok, you got it right? So... what are those things?

To start the more complex thing in this project is `sass/`, inside of it has a lot of sub folders based on [SMACSS](http://smacss.com) methodology, splitting the code, to an easy maintenance, let me make myseft clear:

### SASS structure

  - `abstract/`<br> contains global values, as variables, functions and mixins. Styles that can be used through the whole project.
  - `base/` <br> pre-determinated styles for tags, css reset, pretty munch default styles.
  - `components/` <br> pretty much all the css remains here, remeber: one component equal to one file, inside it has a component styling and a layout styling, components are context aware and were made to be independent. May contains objects and others components in it.
  - `layouts/` <br> used to wrapper things up, in a global way, don't requests specifity. All types of situantions/ one layout equal to one file.
  - `objects/` <br> one object equal to one file, inside it has a object styling and a layout styling, objects aren't context aware and were made to be independent. Mustn't contains components and others objects in it.
  - `states/` <br> temporary states or conditions, basically animations, transitions.
  - `themes/` <br> theme style, one theme equal to one file, dark theme, halloween theme, the components/objects are modify to fit it's own theme purpose.
  - `utilities/` <br> css utilities thats specify certain style to be used in the HTML as classes.

## 🔮 Credits

- [package.json file](https://thinkdobecreate.com/articles/minimum-static-site-sass-setup/)

---

Rcnald thanks you 🧙.
