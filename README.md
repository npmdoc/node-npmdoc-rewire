# api documentation for  [rewire (v2.5.2)](https://github.com/jhnns/rewire)  [![npm package](https://img.shields.io/npm/v/npmdoc-rewire.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-rewire) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-rewire.svg)](https://travis-ci.org/npmdoc/node-npmdoc-rewire)
#### Easy dependency injection for node.js unit testing

[![NPM](https://nodei.co/npm/rewire.png?downloads=true)](https://www.npmjs.com/package/rewire)

[![apidoc](https://npmdoc.github.io/node-npmdoc-rewire/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-rewire_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-rewire/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-rewire/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Johannes Ewald",
        "email": "mail@johannesewald.de"
    },
    "bugs": {
        "url": "https://github.com/jhnns/rewire/issues",
        "email": "mail@johannesewald.de"
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
            "name": "jhnns",
            "email": "mail@johannesewald.de"
        },
        {
            "name": "peerigon",
            "email": "developers@peerigon.com"
        }
    ],
    "name": "rewire",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/jhnns/rewire.git"
    },
    "scripts": {
        "coverage": "istanbul cover ./node_modules/mocha/bin/_mocha",
        "test": "mocha -R spec --check-leaks"
    },
    "version": "2.5.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module rewire](#apidoc.module.rewire)
1.  object <span class="apidocSignatureSpan">rewire.</span>moduleA
1.  object <span class="apidocSignatureSpan">rewire.</span>moduleB
1.  object <span class="apidocSignatureSpan">rewire.</span>moduleEnv
1.  object <span class="apidocSignatureSpan">rewire.</span>strictModule

#### [module rewire.moduleA](#apidoc.module.rewire.moduleA)
1.  [function <span class="apidocSignatureSpan">rewire.moduleA.</span>checkSomeGlobals ()](#apidoc.element.rewire.moduleA.checkSomeGlobals)
1.  [function <span class="apidocSignatureSpan">rewire.moduleA.</span>getBuffer ()](#apidoc.element.rewire.moduleA.getBuffer)
1.  [function <span class="apidocSignatureSpan">rewire.moduleA.</span>getConsole ()](#apidoc.element.rewire.moduleA.getConsole)
1.  [function <span class="apidocSignatureSpan">rewire.moduleA.</span>getDocument ()](#apidoc.element.rewire.moduleA.getDocument)
1.  [function <span class="apidocSignatureSpan">rewire.moduleA.</span>getFilename ()](#apidoc.element.rewire.moduleA.getFilename)
1.  [function <span class="apidocSignatureSpan">rewire.moduleA.</span>getMyNumber ()](#apidoc.element.rewire.moduleA.getMyNumber)
1.  [function <span class="apidocSignatureSpan">rewire.moduleA.</span>getMyObj ()](#apidoc.element.rewire.moduleA.getMyObj)
1.  [function <span class="apidocSignatureSpan">rewire.moduleA.</span>readFileSync ()](#apidoc.element.rewire.moduleA.readFileSync)
1.  [function <span class="apidocSignatureSpan">rewire.moduleA.</span>setMyNumber (newNumber)](#apidoc.element.rewire.moduleA.setMyNumber)
1.  [function <span class="apidocSignatureSpan">rewire.moduleA.</span>setMyObj (newObj)](#apidoc.element.rewire.moduleA.setMyObj)
1.  object <span class="apidocSignatureSpan">rewire.moduleA.</span>someOtherModule

#### [module rewire.moduleB](#apidoc.module.rewire.moduleB)
1.  [function <span class="apidocSignatureSpan">rewire.moduleB.</span>checkSomeGlobals ()](#apidoc.element.rewire.moduleB.checkSomeGlobals)
1.  [function <span class="apidocSignatureSpan">rewire.moduleB.</span>getBuffer ()](#apidoc.element.rewire.moduleB.getBuffer)
1.  [function <span class="apidocSignatureSpan">rewire.moduleB.</span>getConsole ()](#apidoc.element.rewire.moduleB.getConsole)
1.  [function <span class="apidocSignatureSpan">rewire.moduleB.</span>getDocument ()](#apidoc.element.rewire.moduleB.getDocument)
1.  [function <span class="apidocSignatureSpan">rewire.moduleB.</span>getFilename ()](#apidoc.element.rewire.moduleB.getFilename)
1.  [function <span class="apidocSignatureSpan">rewire.moduleB.</span>getMyNumber ()](#apidoc.element.rewire.moduleB.getMyNumber)
1.  [function <span class="apidocSignatureSpan">rewire.moduleB.</span>getMyObj ()](#apidoc.element.rewire.moduleB.getMyObj)
1.  [function <span class="apidocSignatureSpan">rewire.moduleB.</span>readFileSync ()](#apidoc.element.rewire.moduleB.readFileSync)
1.  [function <span class="apidocSignatureSpan">rewire.moduleB.</span>setMyNumber (newNumber)](#apidoc.element.rewire.moduleB.setMyNumber)
1.  [function <span class="apidocSignatureSpan">rewire.moduleB.</span>setMyObj (newObj)](#apidoc.element.rewire.moduleB.setMyObj)
1.  object <span class="apidocSignatureSpan">rewire.moduleB.</span>someOtherModule

#### [module rewire.moduleEnv](#apidoc.module.rewire.moduleEnv)
1.  [function <span class="apidocSignatureSpan">rewire.moduleEnv.</span>inject (prelude, appendix)](#apidoc.element.rewire.moduleEnv.inject)
1.  [function <span class="apidocSignatureSpan">rewire.moduleEnv.</span>load (targetModule)](#apidoc.element.rewire.moduleEnv.load)

#### [module rewire.strictModule](#apidoc.module.rewire.strictModule)
1.  [function <span class="apidocSignatureSpan">rewire.strictModule.</span>doSomethingUnstrict ()](#apidoc.element.rewire.strictModule.doSomethingUnstrict)



# <a name="apidoc.module.rewire"></a>[module rewire](#apidoc.module.rewire)



# <a name="apidoc.module.rewire.moduleA"></a>[module rewire.moduleA](#apidoc.module.rewire.moduleA)

#### <a name="apidoc.element.rewire.moduleA.checkSomeGlobals"></a>[function <span class="apidocSignatureSpan">rewire.moduleA.</span>checkSomeGlobals ()](#apidoc.element.rewire.moduleA.checkSomeGlobals)
- description and source-code
```javascript
function checkSomeGlobals() {
    var isLowerIE,
        typeOfGlobalFunc;

    if (typeof navigator !== "undefined") {
        isLowerIE = /MSIE [6-8]\.[0-9]/g.test(navigator.userAgent);
    }
    if (isLowerIE) {
        typeOfGlobalFunc = "object";
    } else {
        typeOfGlobalFunc = "function";
    }

    if (typeof global !== "object") {
        throw new ReferenceError("global is not an object");
    }
    if (typeof console !== "object") {
        throw new ReferenceError("console is not an object");
    }
    if (typeof require !== "function") {
        throw new ReferenceError("require is not a function");
    }
    if (typeof module !== "object") {
        throw new ReferenceError("module is not an object");
    }
    if (typeof exports !== "object") {
        throw new ReferenceError("exports is not an object");
    }
    if (module.exports !== exports) {
        throw new Error("module.exports === exports returns false");
    }
    if (typeof __dirname !== "string") {
        throw new ReferenceError("__dirname is not a string");
    }
    if (typeof __filename !== "string") {
        throw new ReferenceError("__filename is not a string");
    }
    if (typeof setTimeout !== typeOfGlobalFunc) {
        throw new ReferenceError("setTimeout is not a function");
    }
    if (typeof clearTimeout !== typeOfGlobalFunc) {
        throw new ReferenceError("clearTimeout is not a function");
    }
    if (typeof setInterval !== typeOfGlobalFunc) {
        throw new ReferenceError("setInterval is not a function");
    }
    if (typeof clearInterval !== typeOfGlobalFunc) {
        throw new ReferenceError("clearInterval is not a function");
    }
    if (typeof Error !== "function") {
        throw new ReferenceError("Error is not a function");
    }
    if (typeof parseFloat !== "function") {
        throw new ReferenceError("parseFloat is not a function");
    }
    if (typeof parseInt !== "function") {
        throw new ReferenceError("parseInt is not a function");
    }
    if (typeof window === "undefined") {
        if (typeof process !== "object") {
            throw new ReferenceError("process is not an object");
        }
        if (typeof Buffer !== "function") {
            throw new ReferenceError("Buffer is not a function");
        }
    } else {
        if (typeof encodeURIComponent !== "function") {
            throw new ReferenceError("encodeURIComponent is not a function");
        }
        if (typeof decodeURIComponent !== "function") {
            throw new ReferenceError("decodeURIComponent is not a function");
        }
        if (typeof document !== "object") {
            throw new ReferenceError("document is not an object");
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleA.getBuffer"></a>[function <span class="apidocSignatureSpan">rewire.moduleA.</span>getBuffer ()](#apidoc.element.rewire.moduleA.getBuffer)
- description and source-code
```javascript
function getBuffer() {
    return Buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleA.getConsole"></a>[function <span class="apidocSignatureSpan">rewire.moduleA.</span>getConsole ()](#apidoc.element.rewire.moduleA.getConsole)
- description and source-code
```javascript
function getConsole() {
    return console;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleA.getDocument"></a>[function <span class="apidocSignatureSpan">rewire.moduleA.</span>getDocument ()](#apidoc.element.rewire.moduleA.getDocument)
- description and source-code
```javascript
function getDocument() {
    return document;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleA.getFilename"></a>[function <span class="apidocSignatureSpan">rewire.moduleA.</span>getFilename ()](#apidoc.element.rewire.moduleA.getFilename)
- description and source-code
```javascript
function getFilename() {
    return __filename;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleA.getMyNumber"></a>[function <span class="apidocSignatureSpan">rewire.moduleA.</span>getMyNumber ()](#apidoc.element.rewire.moduleA.getMyNumber)
- description and source-code
```javascript
function getMyNumber() {
    return myNumber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleA.getMyObj"></a>[function <span class="apidocSignatureSpan">rewire.moduleA.</span>getMyObj ()](#apidoc.element.rewire.moduleA.getMyObj)
- description and source-code
```javascript
function getMyObj() {
    return myObj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleA.readFileSync"></a>[function <span class="apidocSignatureSpan">rewire.moduleA.</span>readFileSync ()](#apidoc.element.rewire.moduleA.readFileSync)
- description and source-code
```javascript
function readFileSync() {
    fs.readFileSync("bla.txt", "utf8");
}
```
- example usage
```shell
...
function restoreExtensions() {
    if ("coffee" in originalExtensions) {
        require.extensions[".coffee"] = originalExtensions.coffee;
    }
}

function coffeeExtension(module, filename) {
    var content = stripBOM(fs.readFileSync(filename, "utf8"));

    content = coffee.compile(content, {
        filename: filename,
        bare: true
    });
    module._compile(content, filename);
}
...
```

#### <a name="apidoc.element.rewire.moduleA.setMyNumber"></a>[function <span class="apidocSignatureSpan">rewire.moduleA.</span>setMyNumber (newNumber)](#apidoc.element.rewire.moduleA.setMyNumber)
- description and source-code
```javascript
function setMyNumber(newNumber) {
    myNumber = newNumber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleA.setMyObj"></a>[function <span class="apidocSignatureSpan">rewire.moduleA.</span>setMyObj (newObj)](#apidoc.element.rewire.moduleA.setMyObj)
- description and source-code
```javascript
function setMyObj(newObj) {
    myObj = newObj;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rewire.moduleB"></a>[module rewire.moduleB](#apidoc.module.rewire.moduleB)

#### <a name="apidoc.element.rewire.moduleB.checkSomeGlobals"></a>[function <span class="apidocSignatureSpan">rewire.moduleB.</span>checkSomeGlobals ()](#apidoc.element.rewire.moduleB.checkSomeGlobals)
- description and source-code
```javascript
function checkSomeGlobals() {
    var isLowerIE,
        typeOfGlobalFunc;

    if (typeof navigator !== "undefined") {
        isLowerIE = /MSIE [6-8]\.[0-9]/g.test(navigator.userAgent);
    }
    if (isLowerIE) {
        typeOfGlobalFunc = "object";
    } else {
        typeOfGlobalFunc = "function";
    }

    if (typeof global !== "object") {
        throw new ReferenceError("global is not an object");
    }
    if (typeof console !== "object") {
        throw new ReferenceError("console is not an object");
    }
    if (typeof require !== "function") {
        throw new ReferenceError("require is not a function");
    }
    if (typeof module !== "object") {
        throw new ReferenceError("module is not an object");
    }
    if (typeof exports !== "object") {
        throw new ReferenceError("exports is not an object");
    }
    if (module.exports === exports) {
        throw new Error("module.exports === exports returns true");
    }
    if (typeof __dirname !== "string") {
        throw new ReferenceError("__dirname is not a string");
    }
    if (typeof __filename !== "string") {
        throw new ReferenceError("__filename is not a string");
    }
    if (typeof setTimeout !== typeOfGlobalFunc) {
        throw new ReferenceError("setTimeout is not a function");
    }
    if (typeof clearTimeout !== typeOfGlobalFunc) {
        throw new ReferenceError("clearTimeout is not a function");
    }
    if (typeof setInterval !== typeOfGlobalFunc) {
        throw new ReferenceError("setInterval is not a function");
    }
    if (typeof clearInterval !== typeOfGlobalFunc) {
        throw new ReferenceError("clearInterval is not a function");
    }
    if (typeof Error !== "function") {
        throw new ReferenceError("Error is not a function");
    }
    if (typeof parseFloat !== "function") {
        throw new ReferenceError("parseFloat is not a function");
    }
    if (typeof parseInt !== "function") {
        throw new ReferenceError("parseInt is not a function");
    }
    if (typeof window === "undefined") {
        if (typeof process !== "object") {
            throw new ReferenceError("process is not an object");
        }
        if (typeof Buffer !== "function") {
            throw new ReferenceError("Buffer is not a function");
        }
    } else {
        if (typeof encodeURIComponent !== "function") {
            throw new ReferenceError("encodeURIComponent is not a function");
        }
        if (typeof decodeURIComponent !== "function") {
            throw new ReferenceError("decodeURIComponent is not a function");
        }
        if (typeof document !== "object") {
            throw new ReferenceError("document is not an object");
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleB.getBuffer"></a>[function <span class="apidocSignatureSpan">rewire.moduleB.</span>getBuffer ()](#apidoc.element.rewire.moduleB.getBuffer)
- description and source-code
```javascript
function getBuffer() {
    return Buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleB.getConsole"></a>[function <span class="apidocSignatureSpan">rewire.moduleB.</span>getConsole ()](#apidoc.element.rewire.moduleB.getConsole)
- description and source-code
```javascript
function getConsole() {
    return console;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleB.getDocument"></a>[function <span class="apidocSignatureSpan">rewire.moduleB.</span>getDocument ()](#apidoc.element.rewire.moduleB.getDocument)
- description and source-code
```javascript
function getDocument() {
    return document;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleB.getFilename"></a>[function <span class="apidocSignatureSpan">rewire.moduleB.</span>getFilename ()](#apidoc.element.rewire.moduleB.getFilename)
- description and source-code
```javascript
function getFilename() {
    return __filename;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleB.getMyNumber"></a>[function <span class="apidocSignatureSpan">rewire.moduleB.</span>getMyNumber ()](#apidoc.element.rewire.moduleB.getMyNumber)
- description and source-code
```javascript
function getMyNumber() {
    return myNumber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleB.getMyObj"></a>[function <span class="apidocSignatureSpan">rewire.moduleB.</span>getMyObj ()](#apidoc.element.rewire.moduleB.getMyObj)
- description and source-code
```javascript
function getMyObj() {
    return myObj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleB.readFileSync"></a>[function <span class="apidocSignatureSpan">rewire.moduleB.</span>readFileSync ()](#apidoc.element.rewire.moduleB.readFileSync)
- description and source-code
```javascript
function readFileSync() {
    fs.readFileSync("bla.txt", "utf8");
}
```
- example usage
```shell
...
function restoreExtensions() {
    if ("coffee" in originalExtensions) {
        require.extensions[".coffee"] = originalExtensions.coffee;
    }
}

function coffeeExtension(module, filename) {
    var content = stripBOM(fs.readFileSync(filename, "utf8"));

    content = coffee.compile(content, {
        filename: filename,
        bare: true
    });
    module._compile(content, filename);
}
...
```

#### <a name="apidoc.element.rewire.moduleB.setMyNumber"></a>[function <span class="apidocSignatureSpan">rewire.moduleB.</span>setMyNumber (newNumber)](#apidoc.element.rewire.moduleB.setMyNumber)
- description and source-code
```javascript
function setMyNumber(newNumber) {
    myNumber = newNumber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rewire.moduleB.setMyObj"></a>[function <span class="apidocSignatureSpan">rewire.moduleB.</span>setMyObj (newObj)](#apidoc.element.rewire.moduleB.setMyObj)
- description and source-code
```javascript
function setMyObj(newObj) {
    myObj = newObj;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rewire.moduleEnv"></a>[module rewire.moduleEnv](#apidoc.module.rewire.moduleEnv)

#### <a name="apidoc.element.rewire.moduleEnv.inject"></a>[function <span class="apidocSignatureSpan">rewire.moduleEnv.</span>inject (prelude, appendix)](#apidoc.element.rewire.moduleEnv.inject)
- description and source-code
```javascript
function inject(prelude, appendix) {
    Module.wrapper[0] = moduleWrapper0 + prelude;
    Module.wrapper[1] = appendix + moduleWrapper1;
}
```
- example usage
```shell
...
    // Check if the module uses the strict mode.
    // If so we must ensure that "use strict"; stays at the beginning of the module.
    src = fs.readFileSync(targetPath, "utf8");
    if (detectStrictMode(src) === true) {
        prelude = ' "use strict"; ' + prelude;
    }

    moduleEnv.inject(prelude, appendix);
    moduleEnv.load(targetModule);

    return targetModule.exports;
}

module.exports = internalRewire;
...
```

#### <a name="apidoc.element.rewire.moduleEnv.load"></a>[function <span class="apidocSignatureSpan">rewire.moduleEnv.</span>load (targetModule)](#apidoc.element.rewire.moduleEnv.load)
- description and source-code
```javascript
function load(targetModule) {
    nodeRequire = targetModule.require;
    targetModule.require = requireProxy;
    currentModule = targetModule;

    registerExtensions();
    targetModule.load(targetModule.id);

    // This is only necessary if nothing has been required within the module
    reset();
}
```
- example usage
```shell
...

function load(targetModule) {
nodeRequire = targetModule.require;
targetModule.require = requireProxy;
currentModule = targetModule;

registerExtensions();
targetModule.load(targetModule.id);

// This is only necessary if nothing has been required within the module
reset();
}

function reset() {
Module.wrapper[0] = moduleWrapper0;
...
```



# <a name="apidoc.module.rewire.strictModule"></a>[module rewire.strictModule](#apidoc.module.rewire.strictModule)

#### <a name="apidoc.element.rewire.strictModule.doSomethingUnstrict"></a>[function <span class="apidocSignatureSpan">rewire.strictModule.</span>doSomethingUnstrict ()](#apidoc.element.rewire.strictModule.doSomethingUnstrict)
- description and source-code
```javascript
function doSomethingUnstrict() {
    var caller = arguments.callee.caller;   // this should throw an error as a proof that strict mode is on
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
