<p align="center">
  <a href="http://www.hipsterlogogenerator.com/">
    <img src="https://dl.dropboxusercontent.com/u/6515442/hipsterlogogenerator_1422411720676.png"/>
  </a>
</p>

# Goal
Offer a **fast**, Grunt based, data driven malleable static build system. Use it for any project architecture. 

## Overview
This project seed is cache heavy, smart loading, and mobile first out of the box. [Jade](http://jade-lang.com/) & [Stylus](http://learnboost.github.io/stylus/) are the preprocessor defaults, but swap it for whatever you want, no limits. Want more than 1 preprocessor, it's ready. At the end of the day, it's [Grunt](http://gruntjs.com/), do whatever you want. Add tasks, take care of business.

![Build Status](https://travis-ci.org/argyleink/Bolt.svg?branch=master)
[![Join the chat at https://gitter.im/argyleink/Bolt](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/argyleink/Bolt?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

#### Required
- [Node.js](http://nodejs.org/) and NPM
- [Grunt](http://gruntjs.com/)
- [Bower](http://bower.io/)
- [Bolt CLI](https://github.com/argyleink/Bolt-cli): optional, but handy

#### Quickstart
1. `npm i -g bolt-cli`: very small simple tool to install bolt into directories
2. `bolt new my_site`: my_site should be replaced with your project name
3. `cd bolt-test && npm i && bower i`: install bolt dependencies
4. `grunt`: spin it up!
5. See the [Wiki](https://github.com/argyleink/Bolt/wiki)

## Build Features
- Dev builds are extremely legible, source mapped, and ready for debugging with your tools
- Production builds squish the crap out [images,css,html,js,svg] `grunt --prod`
- Dev and Prod builds have their own output directory, they don't share a `dist/` folder. No need for one build to squash the other.
- Very fast, [concurrent Grunt tasks](https://github.com/argyleink/Bolt/blob/master/tasks/concurrent.coffee), with jit a plugin for really fast watch task running
- Concise [Grunt main file](https://github.com/argyleink/Bolt/blob/master/gruntfile.coffee)
- [Grunt tasks](https://github.com/argyleink/Bolt/tree/master/tasks) are individual, short, easy as hell to read, and a breeze to create
- DRY [Configuration file](https://github.com/argyleink/Bolt/blob/master/app.coffee) keeps project assets and plugins centralized
- [BrowserSync](http://www.browsersync.io) dev server syncs all your clicks, scrolls, and more during development
- BrowserSync live reload and hot css pushes for really rad fast front end crafting
- BrowserSync Weinre remote inspect built in
- Externally accessible server
- Proper [Jade inheritance](https://github.com/paulyoung/jade-inheritance) compilation, so 1 file changed doesn't require the whole project to compile
- Data driven front end development with YAML and/or JSON
- [Auto generated](https://github.com/argyleink/Bolt/blob/master/tasks/manifest.coffee) HTML5 appcache for production builds
- Autoprefixed Stylus
- Git tagging and releasing `grunt bump`
- Easily create custom [build notifications](https://github.com/argyleink/Bolt/blob/master/tasks/notify.coffee)
- Customize your crunched files comment banner
- Ready to run custom [shell commands](https://github.com/argyleink/Bolt/blob/master/tasks/shell.coffee)
- Concurrent image crunching
- [Sublime project file](https://github.com/argyleink/Bolt/blob/master/app.sublime-project) for easy project editing and standards establishment
- Grunt [Heroku](https://github.com/argyleink/Bolt/wiki/Deployments) task for easy CI integration `grunt heroku`
- [CLI](https://github.com/argyleink/Bolt-cli) for easy setup of new projects `bolt new my_app`

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

#### Bolt Extras
- YAML data files are fed directly into your static site template system as JSON
- [Mobile first](https://github.com/argyleink/Bolt/blob/master/app/styles/base/_vars.styl)
- [Flexboxgrid](http://flexboxgrid.com/) library preloaded
- Extensable [Jade page](https://github.com/argyleink/Bolt/blob/master/app/_jade/layouts/page.jade) structure
- Great [Stylus base](https://github.com/argyleink/Bolt/tree/master/app/styles)
- Tons of [mobile header](https://github.com/argyleink/Bolt/tree/master/app/_jade/includes/mobile) and icons, tested and ready
- HTML5 [manifest.json](https://github.com/argyleink/Bolt/blob/master/app/manifest.json)
- 404 page
- [Robots.txt](https://github.com/argyleink/Bolt/blob/master/app/robots.txt)

## Inspiration
- [Roots](http://roots.cx/)
- [Yeoman](http://yeoman.io/)
- [Google Web Starter Kit](https://developers.google.com/web/starter-kit/)
- [HTML5 Mobile Boilerplate](https://github.com/h5bp/html5-boilerplate)
