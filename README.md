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