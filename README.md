# Cordova

### Install corgova
1. Install [Java JDK 8u221](https://www.oracle.com/technetwork/java/javase/downloads/java-archive-javase8u211-later-5573849.html)
2. Install [Node js](https://nodejs.org/)
3. `npm install -g cordova`
4. Download [gradle](https://gradle.org/install/#with-a-package-manager)
5. Extract gradle into folder and add folder to path environment variable

### Create new app
`cordova create <folder> <full-name> <app-name>`
* `folder` on your computer
* `full-name` something like `com.example.hello` (with `<domain>.<publisher>.<folder>`)
* `app-name` the name under the icon on the device

### Add Android platform
`cordova platform add android`

### Build app
`cordova build`

# PWA

### Install precache
`npm install -g sw-precache`

### Configure precache
`sw-precache --config=sw-precache-config.js`

### Install toolbox
`npm install --save sw-toolbox`

### Install localforage
`npm install --save-dev localforage`

### Add workbox
Add `importScripts('https://storage.googleapis.com/workboxcdn/
releases/4.3.1/workbox-sw.js');` into `src/sw.js`

### Inject manifest
`workbox wizard --injectManifest`

### Install http-server
`npm install http-server -g`

### Run server
`http-server ./`

### Build web app
```
cd ./project
npm run build
```

# Express webserver

### Create empty project
`npm init`

### Install Express
`npm install express --save`

### Start server
`node index.js`

OR

`npm start`
* Add `"start": "node index.js"` to package.json

### Install nodemon
`npm install -g nodemon`
* Add `"start": "nodemon index.js"` to package.json

# React

### Install create-react-app
`npm install [-g] create-react-app`
* `-g` install global

### Create classic react app
`create-react-app <app-name>`

### Create TypeScript based react app
`create-react-app <app-name> --template typescript`

### Start development server
`npm start`

### Build for production
`npm run build`

# Angular

### Install angular
`npm install -g @angular/cli`

### Update angular project
```
npm install -g npm-check-updates
npm-check-updates -u
npm install
```

### Create new Angular project
`ng new <project-name>`

### Start developer server
`ng serve [--open]`
* `--open` opens a browser to http://localhost:4200/

### Add component to project
`ng generate component <component-name>`

### Add service to project
`ng generate service <service-name>`

### Add module to project
`ng generate module <module-name> [--flat] [--module=app]`
* `--flat` puts the file in src/app instead of its own folder
* `--module=app` tells the CLI to register it in the imports array of the AppModule

### Add @angular/pwa to existing project
`ng add @angular/pwa --project <project-name>`