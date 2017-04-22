# npmdoc-offline-plugin

#### api documentation for  [offline-plugin (v4.7.0)](https://github.com/NekR/offline-plugin)  [![npm package](https://img.shields.io/npm/v/npmdoc-offline-plugin.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-offline-plugin) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-offline-plugin.svg)](https://travis-ci.org/npmdoc/node-npmdoc-offline-plugin)

#### offline-plugin for webpack

[![NPM](https://nodei.co/npm/offline-plugin.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/offline-plugin)

- [https://npmdoc.github.io/node-npmdoc-offline-plugin/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-offline-plugin/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-offline-plugin/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-offline-plugin/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-offline-plugin/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-offline-plugin/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "offline-plugin",
    "version": "4.7.0",
    "description": "offline-plugin for webpack",
    "main": "lib/index.js",
    "files": [
        "lib/",
        "tpls/",
        "runtime.js",
        "empty-entry.js"
    ],
    "scripts": {
        "test": "node tests/legacy/run && eslint -c configs/eslint.tests.json 'tests/**/**.js'",
        "build": "./node_modules/.bin/babel src/ -d lib/",
        "watch": "npm run build -- --watch",
        "install:build-deps": "node build/install.js",
        "tag": "git push && git push --tags",
        "publish:latest": "npm publish",
        "publish:next": "npm publish --tag=next",
        "release:latest:patch": "npm version patch && npm run tag && npm run publish:latest",
        "release:latest:minor": "npm version minor && npm run tag && npm run publish:latest",
        "release:latest:major": "npm version major && npm run tag && npm run publish:latest",
        "release:next:patch": "npm version patch && npm run tag && npm run publish:next",
        "release:next:minor": "npm version minor && npm run tag && npm run publish:next",
        "release:next:major": "npm version major && npm run tag && npm run publish:next"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/NekR/offline-plugin.git"
    },
    "author": "Arthur Stolyar <nekr.fabula@gmail.com>",
    "license": "MIT",
    "dependencies": {
        "deep-extend": "^0.4.0",
        "ejs": "^2.3.4",
        "loader-utils": "0.2.x",
        "minimatch": "^3.0.3",
        "slash": "^1.0.0"
    },
    "bugs": {
        "url": "https://github.com/NekR/offline-plugin/issues"
    },
    "homepage": "https://github.com/NekR/offline-plugin",
    "keywords": [
        "webpack",
        "plugin",
        "offline",
        "cache",
        "caching",
        "storage",
        "service-worker",
        "serviceworker",
        "appcache",
        "application cache",
        "pwa",
        "progressive web apps",
        "app-shell",
        "appshell"
    ],
    "devDependencies": {
        "chalk": "^1.1.3",
        "cli-highlight": "^1.1.4",
        "del": "^2.2.2",
        "diff": "^3.0.1",
        "dir-compare": "^1.1.0",
        "eslint": "^3.14.1",
        "on-build-webpack": "^0.1.0",
        "webpack": "1.14.0"
    },
    "buildDependencies": {
        "babel": "^5.8.23"
    },
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
