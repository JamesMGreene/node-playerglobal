# node-playerglobal

A Node.js module wrapper for downloading/installing _**ALL**_ versions of the "playerglobal.swc" API library in order to target all modern versions of Flash Player.


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
pg.install(FLEX_HOME);
```