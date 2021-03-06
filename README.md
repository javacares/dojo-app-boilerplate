A Starter Kit for Single Page App
===

- The Dojo App Boilerplate is a set of files to help you rapidly get up and running with the Dojo Toolkit and dapp mvc framework. 
- It illustrates some basic best practices when working with Dojo based on the original work of [dojo-boilerplate](https://github.com/csnover/dojo-boilerplate).
- Helps you build dojo which is some time the most dificult of working with [dojotoolkit](dojotoolkit.org)
- Builds an alternate small build to be embedded in a mobile App like [Apache Cordova/PhoneGap](cordova.io)
- Huge thanks go out to [csnover](https://github.com/csnover) and the other contributors for the original [dojo-boilerplate](https://github.com/csnover/dojo-boilerplate) project. 


Quick Start
-----------

1. Clone the repository using `git clone --recursive https://github.com/csantanapr/dojo-app-boilerplate.git`
2. Develop your project in `src/` until it is amazing.
3. Run `build.sh`, which will create 2 awesome optimized builds `dist/` & `mobile`.
4. Upload `dist/` to a website for millions of people the world over to enjoy.
5. Use `mobile/www` to create an awesome Hybrid Mobile App with [Apache Cordova/PhoneGap](http://cordova.io)
6. Happiness, and stop crying because you can't figure out how to build dojo

### Windows Users

If you have [msysgit](http://git-scm.com) installed, run Git Bash and verify
some dependencies by running the following commands:

    which node

Node will reward you with much faster builds.

A brief tour
------------

* The starting point of the boilerplate is the file at `src/index.html` and `src/app/main.js`  
  It's responsible for loading the Dojo loader and the application’s
  bootstrapper with `config.json`
* The file `build.sh` takes your application files and builds them for
  production use using the Dojo build tool. It depends on the presence of the
  build profile at `profiles/app.profile.js` and App config `src/app/config.json` .
* The App creates an instance of `dojox/app/main` using the App Controller Configuration File  `src/app/config.json`
* The file `src/app/config.json` its the brain to compose the App and also use to figure out dependencies for Dojo Build
* The file `src/app/views/css/app.css` contains import statements to load the CSS it's inserted from `src/index.html` 
* The file `src/app/views/app.js/` is an additional App Controller
* The file `src/app/views/app.html` contains the App level html template and its specified in `src/app/config.json`
* The directories inside `src/app/views/[view1 | view2 | view3]` contain View level module compose of css/images/html/js
* JS = ViewControllers, HTML=ViewTemplates
* Add View Templates, View Controllers, and Object Stores (i.e. Models) starting by modifying the `src/app/config.json`
* The provided directory structure for css, html, and js for your App is defined in config.json, you can change to a different convention

Useful resources
----------------

* [Dojox/App Tutorial](http://dojotoolkit.org/documentation/tutorials/1.9/dojox_app)
* [Dojox/App Reference](http://dojotoolkit.org/reference-guide/dojox/app.html#dojox-app)
* [Dojo Reference Guide](http://dojotoolkit.org/reference-guide/)
* [Dojo API Browser](http://dojotoolkit.org/api/)

About the boilerplate
---------------------

- This project started because I always spent a few weeks getting started with a new version of Dojo, and want to give it a try to the MV* DApp Framework to see how it can be improved.
- This boilerplate is constantly updated to try to reflect the latest and
greatest features and design patterns for developing Single Page Apps with Dojo, but
it relies heavily on information and contributions from other users. 
- If you have an idea, suggestion, or problem, please [report
it](https://github.com/csantanapr/dojo-app-boilerplate/issues) or create a pull
request! (Please note that you will need to have signed the [Dojo
CLA](http://dojofoundation.org/about/cla) before your pull requests are
accepted, for the good of us all!)

Future
---

- Basic boilerplate to create App generator/scaffolding for other projects:
  - [Yoeman](http://yeoman.io)
  - [IBM Worklight](http://ibm.com/mobilefirst)
  - [Apache Cordova CLI](http://cordova.io)
- Examples on how to integrate Dojox/App with other Projects:
  - [Handlebars](http://handlebarsjs.com)
  - [JQuery](http://jquery.com)
  - [Jasmine](http://pivotal.github.com/jasmine)
  - [NodeJS](http://nodejs.org)
  - [MongoDB](http://www.mongodb.org)
- Education resources
  - Screencasts
  - Tutorials
- Next-Gen 2.x
  - [Aura](http://aurajs.com)
  - [BackBoneJS](http://backbonejs.org)
  - [AngularJS](http://angularjs.org)

License
-------

The Dojo App Boilerplate is licensed under the [same
terms](https://github.com/dojo/dojo/blob/master/LICENSE) as the Dojo
Toolkit. Consult the individual projects (see the Useful resources section
above) for additional licensing information.
