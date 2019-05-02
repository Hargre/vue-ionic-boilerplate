# vue-ionic-boilerplate

> A quick boilerplate project for building apps in Ionic 4 using VueJS.


The latest major release of the [Ionic Framework](https://ionicframework.com/) opened up the opportunity for using tools other than Angular for building hybrid mobile applications, including React, Vue and even Vanilla JS. The [Vue version](https://blog.ionicframework.com/announcing-the-ionic-vue-beta/) is still in beta though, and setting up a working project still requires some manual configuration. This boilerplate aims to make this process a bit easier, so you can just try out the framework itself.

## Running the Project

  * #### Clone or download the repo and install its dependencies with your package manager of choice.
  * #### To run the app in the browser:
  ```
  npm run serve
  ```
  * #### To run the app in an emulator/device:
  ```
  ionic cordova run <platform>
  ```
  
  So far this setup has only been tested in Android.
  
## Used Configurations
The project was created via [Vue CLI](https://github.com/vuejs/vue-cli), with the following features enabled:

* Typescript with [class-style components](https://vuejs.org/v2/guide/typescript.html#Class-Style-Vue-Components) + TSLint
* Vue Router
* Vuex
* Sass/SCSS
* Unit testing (Jest)

Cordova is still used for the native bridge, as it makes for a simpler setup at the moment compared to Capacitor, the new bridge in development by the Ionic team.
