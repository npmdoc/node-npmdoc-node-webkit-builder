# npmdoc-node-webkit-builder

#### api documentation for  [node-webkit-builder (v1.0.13)](https://github.com/mllrsohn/node-webkit-builder)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-webkit-builder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-webkit-builder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-webkit-builder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-webkit-builder)

#### node-webkit-builder

[![NPM](https://nodei.co/npm/node-webkit-builder.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/node-webkit-builder)

- [https://npmdoc.github.io/node-npmdoc-node-webkit-builder/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-node-webkit-builder/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-webkit-builder/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-webkit-builder/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-webkit-builder/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-webkit-builder/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Steffen Müller"
    },
    "bin": {
        "nwbuild": "./bin/nwbuild"
    },
    "bugs": {
        "url": "https://github.com/mllrsohn/node-webkit-builder/issues"
    },
    "dependencies": {
        "archiver": "^0.13.0",
        "bluebird": "~1.2.2",
        "decompress-zip": "0.0.8",
        "graceful-fs-extra": "^1.0.4",
        "graceful-ncp": "^2.0.0",
        "inherits": "~2.0.1",
        "lodash": "~2.4.1",
        "optimist": "^0.6.1",
        "platform-overrides": "~1.0.1",
        "plist": "^1.0.0",
        "progress": "~1.1.7",
        "rcedit": "0.2.0",
        "request": "~2.40.0",
        "rimraf": "^2.2.8",
        "semver": "^2.3.1",
        "simple-glob": "~0.1.0",
        "tar-fs": "^0.3.2",
        "temp": "~0.7.0",
        "update-notifier": "^0.1.8",
        "winresourcer": "^0.9.0"
    },
    "deprecated": "WARNING: This module has been renamed to nw-builder. Install using nw-builder instead, node-webkit-builder will no longer be updated.",
    "description": "node-webkit-builder",
    "devDependencies": {
        "colortape": "~0.1.0",
        "nock": "^0.32.3",
        "redtape": "~1.0.0",
        "tape": "~3.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "050a6614263960cb8fd1fa7824911525f2c66b0b",
        "tarball": "https://registry.npmjs.org/node-webkit-builder/-/node-webkit-builder-1.0.13.tgz"
    },
    "gitHead": "896d8cbe7512e80f12114df152c765cc071bd279",
    "homepage": "https://github.com/mllrsohn/node-webkit-builder",
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "steffen"
        },
        {
            "name": "adam-lynch"
        },
        {
            "name": "gabepaez"
        },
        {
            "name": "dylangattey"
        },
        {
            "name": "trevorah"
        }
    ],
    "name": "node-webkit-builder",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/mllrsohn/node-webkit-builder.git"
    },
    "scripts": {
        "test": "colortape test/*.js"
    },
    "version": "1.0.13"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
