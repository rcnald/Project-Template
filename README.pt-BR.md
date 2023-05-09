<h1 align="center">Project Template</h1>

[![pt-BR](https://img.shields.io/badge/language-pt--BR-green)](https://github.com/rcnald/Project-Template/blob/main/README.pt-BR.md)
[![en-US](https://img.shields.io/badge/language-en--US-gray)](https://github.com/rcnald/Project-Template/blob/main/README.md)

## ♾️ Requisitos

- [Node.js](https://nodejs.org/en/download/)


## ⚗️ Tecnologias

Este projeto usou as seguintes tecnologias:

<p align="left">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <img src="https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=sass&logoColor=white">
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white">
</p>

## 👨‍💻 Como usar

| linha de comando | oque faz                            | OBS                        |
|------------------|-------------------------------------|----------------------------|
| npm install      | instala dependencias(node_modules)  | executar primeiro, uma vez |
| npm start        | executa live:server,sass & tailwind | em produção                |
| npm run build    | executa autoprefixer                | projeto finalizado         |

**npm install** deve ser executado quando você git clone (baixar) o arquivo para gerar a pasta 'node_modules', dentro todas as dependências para rodar as tecnologias.

**npm start** ele inicia, sass, tailwindcs live-compiler e live-server na porta [localhost:3000](https://localhost:3000). Os arquivos compilados estarão na pasta 'dist' (somente escreva códigos na pasta 'src').

**npm run build** quando o projeto é concluído, ele compila novamente, apenas o arquivo dist/css, e executa o plug-in autoprefixer que evita problemas entre navegadores.

## 🤔 Como faço para codar?

Você pode se questionar, o que são aquelas coisas de 'letra-{nome}' nas classes de HTML? Chama-se [Namespaces](https://csswizardry.com/2015/03/more-transparent-ui-code-with-namespaces/), sua função é informar o tipo do elemento e onde encontra-lo apenas por vê-lo. Eu particularmente uso estes:
  - `o-` - object
  - `c-` - component
  - `l-` - layout
  - `u-` - utilities
  - `t-` - themes
  - `is-/has-` - states
  - `js-` - DOM elements

...Ok, entendeu? Então... o que são essas coisas?

Para começar o mais complexo desse projeto é o `sass/`, dentro dele tem várias subpastas baseadas na metodologia [SMACSS](http://smacss.com), dividindo o código, para uma fácil manutenção, deixe-me esclarecer:

### estrutura SASS

  - `abstract/`<br> contém valores globais, como variáveis, funções e mixins. Estilos que podem ser usados ​​em todo o projeto.
  - `base/` <br> stilos pré-determinados para tags, redefinição de css, muitos estilos padrão.
  - `components/` <br> praticamente todo o css fica aqui, lembre-se: um componente igual a um arquivo, dentro dele tem um estilo de componente e um estilo de layout, os componentes são sensíveis ao contexto e foram feitos para serem independentes. podem conter objetos e outros componentes nele.
  - `layouts/` <br> usado para agrupar as coisas, de forma global, não solicita especificidade. Todos os tipos de situações/ um layout igual a um arquivo.
  - `objects/` <br> um objeto é igual a um arquivo, dentro dele tem um estilo de objeto e um estilo de layout, os objetos não são sensíveis ao contexto e foram feitos para serem independentes. Não deve conter componentes e outros objetos nele.
  - `states/` <br> estados ou condições temporárias, basicamente animações, transições.
  - `themes/` <br> estilo do tema, um tema igual a um arquivo, tema escuro, tema do dia das bruxas, os componentes/objetos são modificados para atender ao propósito do tema.
  - `utilities/` <br> utilitários css que especificam certo estilo a ser usado no HTML como classes.

## 🔮 Creditos

- [arquivo package.json](https://thinkdobecreate.com/articles/minimum-static-site-sass-setup/)

---

Rcnald agradece 🧙.
