[![Build Status](https://travis-ci.org/JamesMGreene/node-playerglobal.png?branch=master)](https://travis-ci.org/JamesMGreene/node-playerglobal)

# node-playerglobal

A Node.js module wrapper for downloading/installing _**ALL**_ versions of the "playerglobal.swc" API library in order to target all modern versions of Flash Player.

If you would prefer to be able to always have the latest versions without this waiting for this module to be updated and re-published, check out [JamesMGreene/node-playerglobal-latest](https://github.com/JamesMGreene/node-playerglobal-latest) instead.


## Install

```shell
npm install playerglobal
```


## Usage

```js
var pg = require('playerglobal');

console.log('PlayerGlobal root path: ' + pg.path);

// Install the PlayerGlobal dir into a Flex SDK dir
var FLEX_HOME = process.env['FLEX_HOME'] || __dirname;
pg.install(FLEX_HOME, function(err) {
  if (err) {
    console.error('Failed to install the Flash API libraries!\nError: ' + err);
  }
});
```
