# Angular WebPack Starter
Seed project to start ES6, Angular 1.5, ngNewRouter, Webpack, WebPack Dev Server, & NodeJS tested via karma-jasmine & cucumber.

NB: there is no `gulp` or `grunt`, but some `bash` scripts for task automation support.

**You can view the live example here:  [View Live Example](http://angular-webpack-starter.herokuapp.com)**


How can I install it?
============
1) Get the library:

**Download from Github and cd into it**

```
$ git clone https://github.com/JustinWinthers/angular-webpack-starter.git
$ cd angular-webpack-starter
```

2) Install the Node Version Manager [nvm](https://github.com/creationix/nvm/blob/master/README.markdown)
   and [direnv](http://direnv.net).

Create ~/.direnvrc with the following contents:

    #!/usr/bin/env bash
    set -e

    nvm() {
        . ~/.nvm/nvm.sh
        nvm "$@"
    }

This will allow us to call `nvm use` in the `.envrc` file in the project's dir, which will consult the version specified in the `.nvmrc` file to switch to that version of node for the project.

NB1: if the version in the `nvmrc` is not yet installed, run `nvm install`.

NB2: after `.envrc` calls `nvm` to activate the relevant node version, it will append `node_modules/.bin` and `bin` to the path.

2) Install all of the node `dependencies` and `devDependencies`

**NB: Avoid installing global dependencies so as to keep each project completely independent.**

```
npm install
```

3.) start the webpack dev server

**Run the server from the command line by typing:**

```
npm start
```

5.)  Navigate to http://localhost:8080/#/


## For deployments

Type ```webpack``` on the command line to build the bundle.js as the WebPack Dev Server deploys only an in memory
copy of bundle.js that satisfies get requests when running the server.

## Authors

**Justin Winthers**

+ https://github.com/JustinWinthers

**Lachlan Deck**

+ https://github.com/ldeck

## Thanks

+ https://github.com/JustinWinthers/angular-webpack-starter
+ https://github.com/halversondm/webpack-express-angular
+ https://github.com/preboot/angular-webpack

## License

Copyright 2014 Digital Advisors, LLC

Licensed under the Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
