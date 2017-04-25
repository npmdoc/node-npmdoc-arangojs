# npmdoc-arangojs

#### basic api documentation for  [arangojs (v5.6.1)](https://github.com/arangodb/arangojs)  [![npm package](https://img.shields.io/npm/v/npmdoc-arangojs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-arangojs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-arangojs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-arangojs)

#### The official ArangoDB JavaScript driver.

[![NPM](https://nodei.co/npm/arangojs.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/arangojs)

- [https://npmdoc.github.io/node-npmdoc-arangojs/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-arangojs/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-arangojs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-arangojs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-arangojs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-arangojs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "ArangoDB GmbH"
    },
    "browser": {
        "./lib/util/btoa.js": "./lib/util/btoa.web.js",
        "./lib/util/bytelength.js": "./lib/util/bytelength.web.js",
        "./lib/util/multipart.js": "./lib/util/multipart.web.js",
        "./lib/util/request.js": "./lib/util/request.web.js"
    },
    "bugs": {
        "url": "https://github.com/arangodb/arangojs/issues"
    },
    "contributors": [
        {
            "name": "Alan Plum"
        }
    ],
    "dependencies": {
        "es6-error": "^4.0.1",
        "http-errors": "^1.6.1",
        "linkedlist": "^1.0.1",
        "multi-part": "^2.0.0",
        "retry": "^0.10.0",
        "utf8-length": "^0.0.1",
        "xhr": "^2.3.1"
    },
    "description": "The official ArangoDB JavaScript driver.",
    "devDependencies": {
        "babel-cli": "6.24.0",
        "babel-core": "6.24.0",
        "babel-loader": "6.4.1",
        "babel-plugin-add-module-exports": "0.2.1",
        "babel-plugin-transform-builtin-extend": "1.1.2",
        "babel-plugin-transform-es2015-modules-commonjs": "6.24.0",
        "babel-preset-es2015": "6.24.0",
        "babel-preset-stage-1": "6.22.0",
        "chai": "3.5.0",
        "core-js": "2.4.1",
        "coveralls": "2.13.0",
        "istanbul": "0.4.5",
        "json-loader": "0.5.4",
        "mocha": "3.2.0",
        "npm-run-all": "4.0.2",
        "snazzy": "7.0.0",
        "standard": "10.0.0",
        "watch": "1.0.2",
        "webpack": "1.14.0",
        "xunit-file": "1.0.0"
    },
    "directories": {
        "lib": "lib"
    },
    "dist": {
        "shasum": "c51ca877f9d24e0796877528ca82cbecdb279c42",
        "tarball": "https://registry.npmjs.org/arangojs/-/arangojs-5.6.1.tgz"
    },
    "files": [
        "lib/",
        "package.json",
        "arangojs.d.ts",
        "README.md",
        "LICENSE"
    ],
    "gitHead": "125db50c3d5d71d44fa73598e0ae16e6fbe445da",
    "homepage": "https://github.com/arangodb/arangojs",
    "keywords": [
        "arango",
        "arangodb",
        "aql",
        "nosql",
        "client",
        "driver",
        "api",
        "http",
        "rest"
    ],
    "license": "Apache-2.0",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "fceller"
        },
        {
            "name": "jsteemann"
        },
        {
            "name": "mpv1989"
        },
        {
            "name": "pluma"
        }
    ],
    "name": "arangojs",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/arangodb/arangojs.git"
    },
    "scripts": {
        "ci": "mocha",
        "dist": "npm-run-all -p dist:*",
        "dist:browser": "webpack",
        "dist:node": "babel --compact false -d lib src",
        "jenkins": "npm run ci -- --timeout 0 --reporter xunit-file",
        "lint": "standard --verbose src/**/*.js test/**/*.js | snazzy",
        "preci": "npm install",
        "prepublish": "npm run lint && npm run dist && node -e 'require(\"./\");'",
        "test": "mocha --growl",
        "watch": "npm-run-all -p watch:*",
        "watch:browser": "npm run dist:browser -- --watch",
        "watch:node": "watch 'npm run dist:node' ./src ./test",
        "watch:test": "watch 'npm run lint && npm run test' ./src ./test"
    },
    "typings": "arangojs.d.ts",
    "version": "5.6.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
