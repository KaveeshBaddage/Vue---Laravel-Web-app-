# Vue---Laravel-Web-app-
A web application use Vue ,a progressive framework for building user interfaces and Laravel , open-source PHP web framework

#Vue

### Install Vue framework

NPM is the recommended installation method when building large scale applications with Vue. <br/>

    npm install vue

Vue.js provides an official CLI for quickly scaffolding ambitious Single Page Applications.. It takes only a few minutes to get up and running with hot-reload, lint-on-save, and production-ready builds:

#### install vue-cli
     npm install --global vue-cli

#### create a new project using the "webpack" template
    $ vue init webpack webapp


    ? Project name (webapp) webapp
    ? Project name webapp
    ? Project description (A Vue.js project) Web Application
    ? Project description Web Applicarion
    ? Author Kaveesha Baddage
    ? Author Kaveesha Baddage
    ? Vue build (Use arrow keys)
    > Runtime + Compiler: recommended for most users
    ? Vue build standalone
    ? Install vue-router? (Y/n) Y
    ? Install vue-router? Yes
    ? Use ESLint to lint your code? (Y/n) Y
    ? Use ESLint to lint your code? Yes
    ? Pick an ESLint preset (Use arrow keys)
    ? Pick an ESLint preset Standard
    ? Set up unit tests (Y/n) n
    ? Set up unit tests No
    ? Setup e2e tests with Nightwatch? (Y/n) n
    ? Setup e2e tests with Nightwatch? No
    ? Should we run `npm install` for you after the project has been created? (reco
    ? Should we run `npm install` for you after the project has been created? (reco
    mmended) npm

###### install dependencies
    npm install

###### serve with hot reload at localhost:8080
    npm run dev

###### build for production with minification
    npm run build

###### build for production and view the bundle analyzer report
    npm run build --report


For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader). <br/>

### Install the Vue Devtools in Chrome browser
    https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd/

##### Webpack 
webpack is a module bundler. Its main purpose is to bundle JavaScript files for usage in a browser, yet it is also capable of transforming, bundling, or packaging just about any resource or asset.<br/>

For a basic example, imagine we have a bunch of CommonJS modules. They cannot run directly inside the browser, so we need to "bundle" them into a single file that can be included via a <script> tag. webpack can follow the dependencies of the require() calls and do that for us.

##### Vue Loader 
vue-loader is a loader for webpack that can transform Vue components written in the standard format into a plain JavaScript module:<br/>

`In a nutshell, the combination of webpack and vue-loader gives you a modern, flexible and extremely powerful front-end workflow for authoring Vue.js applications.`




