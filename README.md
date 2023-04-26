<h1 align="center">Project Template</h1>

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

To start the more complex thing is here in `sass/`, inside of it has a lot of sub folders based on [SMACSS](http://smacss.com) methodology, splitting the code, to an 
easy maintenance, let me make myseft clear:

### src/sass structure

  - `abstract/` - contains variables and global style, like functions and mixins.
  - `base/` - css reset, default styles.
  - `components/` - pretty much all the css remains here, remeber: one component equal to one file, inside it has a component styling and a layout styling, usually contains objects and others components in it; context aware.
  - `layouts/` - used to wrapper things up, in a global way.
  - `objects/` - almost the same thing as components, but don't accept other objects or components other than itself.
  - `states/` - animations.
  - `themes/` - theme style, darkmode, halloween theme...
  - `utilities/` - utilities to be used in HTML as classes.

## 🔮 Credits

- [package.json file](https://thinkdobecreate.com/articles/minimum-static-site-sass-setup/)

---

Rcnald thanks you 🧙.
