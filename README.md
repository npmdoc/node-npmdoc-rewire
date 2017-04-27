# npmdoc-rewire

#### basic api documentation for  [rewire (v2.5.2)](https://github.com/jhnns/rewire)  [![npm package](https://img.shields.io/npm/v/npmdoc-rewire.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-rewire) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-rewire.svg)](https://travis-ci.org/npmdoc/node-npmdoc-rewire)

#### Easy dependency injection for node.js unit testing

[![NPM](https://nodei.co/npm/rewire.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/rewire)

- [https://npmdoc.github.io/node-npmdoc-rewire/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-rewire/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-rewire/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-rewire/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-rewire/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-rewire/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Johannes Ewald"
    },
    "bugs": {
        "url": "https://github.com/jhnns/rewire/issues"
    },
    "dependencies": {},
    "description": "Easy dependency injection for node.js unit testing",
    "devDependencies": {
        "coffee-script": "^1.8.0",
        "expect.js": "^0.3.1",
        "mocha": "^2.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "6427de7b7feefa7d36401507eb64a5385bc58dc7",
        "tarball": "https://registry.npmjs.org/rewire/-/rewire-2.5.2.tgz"
    },
    "gitHead": "fff5037950f78b4164c299560f761bd5e3dc9e06",
    "homepage": "https://github.com/jhnns/rewire",
    "keywords": [
        "dependency",
        "injection",
        "mock",
        "shim",
        "module",
        "unit",
        "test",
        "leak",
        "inspect",
        "fake",
        "require"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "jhnns"
        },
        {
            "name": "peerigon"
        }
    ],
    "name": "rewire",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/jhnns/rewire.git"
    },
    "scripts": {
        "coverage": "istanbul cover ./node_modules/mocha/bin/_mocha",
        "test": "mocha -R spec --check-leaks"
    },
    "version": "2.5.2",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
