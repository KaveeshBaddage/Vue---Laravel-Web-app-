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

## Flow of the redering content

In `index.html`, it contains following code snip. App component will me mounted here.<br/>

    <body>
        <div id="app"></div>
        <!-- built files will be auto injected -->
    </body>

In `main.js` it create a new Vue instance. <br/>

    new Vue({
    el: '#app',
    router,
    components: { App },
    template: '<App/>'
    })

In `App.vue` it defines a template that will be render as app component. <br/>

    <template>
    <div id="app">
        <!-- <img src="./assets/logo.png"> -->
        <router-view/>
    </div>
    </template>

Here  <router-view/> will add all the routing path and components reagarding to that routes.<br/>

In `router/index.js` defines all routes in a array.<br/>

    routes: [
        {
        path: '/',
        name: 'HelloWorld',
        component: HelloWorld
        },
        {
        path: '/dashboard',
        name: 'Dashboard',
        component: Dashboard
        }
    ]

### Add front-end CSS library — Bootstrap V4.

    npm i bootstrap-vue

Then, register BootstrapVue plugin in your app entry point(router/index.js)<br/>

    import BootstrapVue from 'bootstrap-vue'
    Vue.use(BootstrapVue);

And import Bootstrap and Bootstrap-Vue css files:<br/>

    import 'bootstrap/dist/css/bootstrap.css'
    import 'bootstrap-vue/dist/bootstrap-vue.css'

### Remove front-end CSS library — Bootstrap V4 from project and also removes it from dependencies in package.json.

    npm uninstall bootstrap-vue --save


### Add Vuetify progressive framework 

    npm install vuetify --save

### Import Vuetify and tell Vue to use it

In most cases this will be index.js or main.js<br/>

    import Vue from 'vue'
    import Vuetify from 'vuetify'
 
    Vue.use(Vuetify)


include the Vuetify css file. Simply include the Vuetify css file in your index.html or import the actual stylus file or the minified css.<br/>

    // index.js or main.js
    import 'vuetify/dist/vuetify.min.css'

The easiest way to include the Material Design icons is to add a link tag to your index.html file.<br/>

    <head>
    <link href='https://fonts.googleapis.com/css?family=Roboto:300,400,500,700|Material+Icons' rel="stylesheet">
    </head>

### Vue Components

Here is a vue component<br/>

    `// Define a new component called button-counter
    Vue.component('button-counter', {
    data: function () {
        return {
        count: 0
        }
    },
    template: '<button v-on:click="count++">You clicked me {{ count }} times.</button>'
    })`

Component can be used as follows<br/>

    <div id="components-demo">
    <button-counter></button-counter>
    </div>

Component `data` must be function. If it is not we cannot use same component in many times. Because every reused component will refer same object. A component’s data option must be a function to avoid that. So that each instance can maintain an independent copy of the returned data object.<br/>



