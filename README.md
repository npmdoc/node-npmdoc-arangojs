# api documentation for  [arangojs (v5.6.0)](https://github.com/arangodb/arangojs)  [![npm package](https://img.shields.io/npm/v/npmdoc-arangojs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-arangojs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-arangojs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-arangojs)
#### The official ArangoDB JavaScript driver.

[![NPM](https://nodei.co/npm/arangojs.png?downloads=true)](https://www.npmjs.com/package/arangojs)

[![apidoc](https://npmdoc.github.io/node-npmdoc-arangojs/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-arangojs%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-arangojs/build/apidoc.html)

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
            "name": "Alan Plum",
            "email": "me@pluma.io"
        }
    ],
    "dependencies": {
        "es6-error": "^4.0.1",
        "http-errors": "^1.5.0",
        "linkedlist": "^1.0.1",
        "multi-part": "^2.0.0",
        "retry": "^0.10.0",
        "utf8-length": "^0.0.1",
        "xhr": "^2.3.1"
    },
    "description": "The official ArangoDB JavaScript driver.",
    "devDependencies": {
        "babel-cli": "6.22.2",
        "babel-core": "6.22.1",
        "babel-loader": "6.2.9",
        "babel-plugin-add-module-exports": "0.2.1",
        "babel-plugin-transform-builtin-extend": "1.1.0",
        "babel-plugin-transform-es2015-modules-commonjs": "6.22.0",
        "babel-preset-es2015": "6.22.0",
        "babel-preset-stage-1": "6.22.0",
        "chai": "3.5.0",
        "core-js": "2.4.1",
        "coveralls": "2.11.15",
        "istanbul": "0.4.5",
        "json-loader": "0.5.4",
        "mocha": "3.2.0",
        "npm-run-all": "4.0.1",
        "snazzy": "6.0.0",
        "standard": "8.6.0",
        "watch": "1.0.1",
        "webpack": "1.14.0"
    },
    "directories": {
        "lib": "lib"
    },
    "dist": {
        "shasum": "89f2d9321462c9f99b22e916a26502e03620666c",
        "tarball": "https://registry.npmjs.org/arangojs/-/arangojs-5.6.0.tgz"
    },
    "files": [
        "lib/",
        "package.json",
        "arangojs.d.ts",
        "README.md",
        "LICENSE"
    ],
    "gitHead": "e43bfc6df6e8d41607dc1978edabc883303bd4a9",
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
            "name": "fceller",
            "email": "frank@arangodb.com"
        },
        {
            "name": "jsteemann",
            "email": "jsteemann@mail.ru"
        },
        {
            "name": "mpv1989",
            "email": "mark@arangodb.com"
        },
        {
            "name": "pluma",
            "email": "me@pluma.io"
        }
    ],
    "name": "arangojs",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/arangodb/arangojs.git"
    },
    "scripts": {
        "ci": "mocha",
        "dist": "npm-run-all -p dist:*",
        "dist:browser": "webpack",
        "dist:node": "babel --compact false -d lib src",
        "lint": "snazzy --verbose src/**/*.js test/**/*.js",
        "prepublish": "npm run lint && npm run dist && node -e 'require(\"./\");'",
        "test": "mocha --growl",
        "watch": "npm-run-all -p watch:*",
        "watch:browser": "npm run dist:browser -- --watch",
        "watch:node": "watch 'npm run dist:node' ./src ./test",
        "watch:test": "watch 'npm run lint && npm run test' ./src ./test"
    },
    "typings": "arangojs.d.ts",
    "version": "5.6.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module arangojs](#apidoc.module.arangojs)
1.  [function <span class="apidocSignatureSpan">arangojs.</span>Database (config)](#apidoc.element.arangojs.Database)
1.  [function <span class="apidocSignatureSpan">arangojs.</span>aql (strings)](#apidoc.element.arangojs.aql)
1.  [function <span class="apidocSignatureSpan">arangojs.</span>aqlQuery (strings)](#apidoc.element.arangojs.aqlQuery)
1.  object <span class="apidocSignatureSpan">arangojs.</span>aql_query
1.  object <span class="apidocSignatureSpan">arangojs.</span>collection
1.  object <span class="apidocSignatureSpan">arangojs.</span>connection
1.  object <span class="apidocSignatureSpan">arangojs.</span>cursor
1.  object <span class="apidocSignatureSpan">arangojs.</span>database
1.  object <span class="apidocSignatureSpan">arangojs.</span>error
1.  object <span class="apidocSignatureSpan">arangojs.</span>graph
1.  object <span class="apidocSignatureSpan">arangojs.</span>route

#### [module arangojs.aql_query](#apidoc.module.arangojs.aql_query)
1.  [function <span class="apidocSignatureSpan">arangojs.aql_query.</span>default (strings)](#apidoc.element.arangojs.aql_query.default)

#### [module arangojs.collection](#apidoc.module.arangojs.collection)
1.  [function <span class="apidocSignatureSpan">arangojs.collection.</span>DocumentCollection ()](#apidoc.element.arangojs.collection.DocumentCollection)
1.  [function <span class="apidocSignatureSpan">arangojs.collection.</span>EdgeCollection ()](#apidoc.element.arangojs.collection.EdgeCollection)
1.  [function <span class="apidocSignatureSpan">arangojs.collection.</span>_BaseCollection (connection, name)](#apidoc.element.arangojs.collection._BaseCollection)
1.  [function <span class="apidocSignatureSpan">arangojs.collection.</span>default (connection, body)](#apidoc.element.arangojs.collection.default)
1.  object <span class="apidocSignatureSpan">arangojs.collection.</span>_types
1.  object <span class="apidocSignatureSpan">arangojs.collection.</span>types

#### [module arangojs.connection](#apidoc.module.arangojs.connection)
1.  [function <span class="apidocSignatureSpan">arangojs.connection.</span>default (config)](#apidoc.element.arangojs.connection.default)

#### [module arangojs.cursor](#apidoc.module.arangojs.cursor)
1.  [function <span class="apidocSignatureSpan">arangojs.cursor.</span>default (connection, body)](#apidoc.element.arangojs.cursor.default)

#### [module arangojs.database](#apidoc.module.arangojs.database)
1.  [function <span class="apidocSignatureSpan">arangojs.database.</span>default (config)](#apidoc.element.arangojs.database.default)

#### [module arangojs.error](#apidoc.module.arangojs.error)
1.  [function <span class="apidocSignatureSpan">arangojs.error.</span>default (obj)](#apidoc.element.arangojs.error.default)

#### [module arangojs.graph](#apidoc.module.arangojs.graph)
1.  [function <span class="apidocSignatureSpan">arangojs.graph.</span>EdgeCollection (connection, name, graph)](#apidoc.element.arangojs.graph.EdgeCollection)
1.  [function <span class="apidocSignatureSpan">arangojs.graph.</span>VertexCollection (connection, name, graph)](#apidoc.element.arangojs.graph.VertexCollection)
1.  [function <span class="apidocSignatureSpan">arangojs.graph.</span>default (connection, name)](#apidoc.element.arangojs.graph.default)

#### [module arangojs.route](#apidoc.module.arangojs.route)
1.  [function <span class="apidocSignatureSpan">arangojs.route.</span>default (connection, path, headers)](#apidoc.element.arangojs.route.default)



# <a name="apidoc.module.arangojs"></a>[module arangojs](#apidoc.module.arangojs)

#### <a name="apidoc.element.arangojs.Database"></a>[function <span class="apidocSignatureSpan">arangojs.</span>Database (config)](#apidoc.element.arangojs.Database)
- description and source-code
```javascript
function Database(config) {
  _classCallCheck(this, Database);

  this._connection = new _connection2.default(config);
  this._api = this._connection.route('/_api');
  this.name = this._connection.config.databaseName;
}
```
- example usage
```shell
...
let db1 = arangojs(); // convenience short-hand
let db2 = new Database();
let result = await db2.query(aql'RETURN ${Date.now()}');

// or plain old Node-style
var arangojs = require('arangojs');
var db1 = arangojs();
var db2 = new arangojs.Database();
db2.query(
{
  query: 'RETURN @arg0',
  bindVars: {arg0: Date.now()}
},
function (err, result) {
  // ...
...
```

#### <a name="apidoc.element.arangojs.aql"></a>[function <span class="apidocSignatureSpan">arangojs.</span>aql (strings)](#apidoc.element.arangojs.aql)
- description and source-code
```javascript
function aql(strings) {
  var bindVars = {};
  var bindVals = [];
  var query = strings[0];

  for (var _len = arguments.length, args = Array(_len > 1 ? _len - 1 : 0), _key = 1; _key < _len; _key++) {
    args[_key - 1] = arguments[_key];
  }

  for (var i = 0; i < args.length; i++) {
    var rawValue = args[i];
    var value = rawValue;
    if (rawValue && typeof rawValue.toAQL === 'function') {
      query += '' + rawValue.toAQL() + strings[i + 1];
      continue;
    }
    var index = bindVals.indexOf(rawValue);
    var isKnown = index !== -1;
    var name = 'value' + (isKnown ? index : bindVals.length);
    if (rawValue && rawValue.isArangoCollection) {
      name = '@' + name;
      value = rawValue.name;
    }
    if (!isKnown) {
      bindVals.push(rawValue);
      bindVars[name] = value;
    }
    query += '@' + name + strings[i + 1];
  }
  return { query: query, bindVars: bindVars };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.arangojs.aqlQuery"></a>[function <span class="apidocSignatureSpan">arangojs.</span>aqlQuery (strings)](#apidoc.element.arangojs.aqlQuery)
- description and source-code
```javascript
function aql(strings) {
  var bindVars = {};
  var bindVals = [];
  var query = strings[0];

  for (var _len = arguments.length, args = Array(_len > 1 ? _len - 1 : 0), _key = 1; _key < _len; _key++) {
    args[_key - 1] = arguments[_key];
  }

  for (var i = 0; i < args.length; i++) {
    var rawValue = args[i];
    var value = rawValue;
    if (rawValue && typeof rawValue.toAQL === 'function') {
      query += '' + rawValue.toAQL() + strings[i + 1];
      continue;
    }
    var index = bindVals.indexOf(rawValue);
    var isKnown = index !== -1;
    var name = 'value' + (isKnown ? index : bindVals.length);
    if (rawValue && rawValue.isArangoCollection) {
      name = '@' + name;
      value = rawValue.name;
    }
    if (!isKnown) {
      bindVals.push(rawValue);
      bindVars[name] = value;
    }
    query += '@' + name + strings[i + 1];
  }
  return { query: query, bindVars: bindVars };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.arangojs.aql_query"></a>[module arangojs.aql_query](#apidoc.module.arangojs.aql_query)

#### <a name="apidoc.element.arangojs.aql_query.default"></a>[function <span class="apidocSignatureSpan">arangojs.aql_query.</span>default (strings)](#apidoc.element.arangojs.aql_query.default)
- description and source-code
```javascript
function aql(strings) {
  var bindVars = {};
  var bindVals = [];
  var query = strings[0];

  for (var _len = arguments.length, args = Array(_len > 1 ? _len - 1 : 0), _key = 1; _key < _len; _key++) {
    args[_key - 1] = arguments[_key];
  }

  for (var i = 0; i < args.length; i++) {
    var rawValue = args[i];
    var value = rawValue;
    if (rawValue && typeof rawValue.toAQL === 'function') {
      query += '' + rawValue.toAQL() + strings[i + 1];
      continue;
    }
    var index = bindVals.indexOf(rawValue);
    var isKnown = index !== -1;
    var name = 'value' + (isKnown ? index : bindVals.length);
    if (rawValue && rawValue.isArangoCollection) {
      name = '@' + name;
      value = rawValue.name;
    }
    if (!isKnown) {
      bindVals.push(rawValue);
      bindVars[name] = value;
    }
    query += '@' + name + strings[i + 1];
  }
  return { query: query, bindVars: bindVars };
}
```
- example usage
```shell
...
    }

    var _connection$promisify12 = this._connection.promisify(cb),
        promise = _connection$promisify12.promise,
        callback = _connection$promisify12.callback;

    this._api.put('/simple/all', _extends({}, opts, { collection: this.name }), function (err, res) {
      return err ? callback(err) : callback(null, new _cursor2.default(_this2._connection, res.body));
    });
    return promise;
  }
}, {
  key: 'any',
  value: function any(cb) {
    var _connection$promisify13 = this._connection.promisify(cb),
...
```



# <a name="apidoc.module.arangojs.collection"></a>[module arangojs.collection](#apidoc.module.arangojs.collection)

#### <a name="apidoc.element.arangojs.collection.DocumentCollection"></a>[function <span class="apidocSignatureSpan">arangojs.collection.</span>DocumentCollection ()](#apidoc.element.arangojs.collection.DocumentCollection)
- description and source-code
```javascript
function DocumentCollection() {
  var _ref;

  _classCallCheck(this, DocumentCollection);

  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  var _this5 = _possibleConstructorReturn(this, (_ref = DocumentCollection.__proto__ || Object.getPrototypeOf(DocumentCollection
)).call.apply(_ref, [this].concat(args)));

  _this5.type = types.DOCUMENT_COLLECTION;
  return _this5;
}
```
- example usage
```shell
...
  }

  // Collection manipulation

}, {
  key: 'collection',
  value: function collection(collectionName) {
    return new _collection.DocumentCollection(this._connection, collectionName);
  }
}, {
  key: 'edgeCollection',
  value: function edgeCollection(collectionName) {
    return new _collection.EdgeCollection(this._connection, collectionName);
  }
}, {
...
```

#### <a name="apidoc.element.arangojs.collection.EdgeCollection"></a>[function <span class="apidocSignatureSpan">arangojs.collection.</span>EdgeCollection ()](#apidoc.element.arangojs.collection.EdgeCollection)
- description and source-code
```javascript
function EdgeCollection() {
  var _ref2;

  _classCallCheck(this, EdgeCollection);

  for (var _len2 = arguments.length, args = Array(_len2), _key2 = 0; _key2 < _len2; _key2++) {
    args[_key2] = arguments[_key2];
  }

  var _this6 = _possibleConstructorReturn(this, (_ref2 = EdgeCollection.__proto__ || Object.getPrototypeOf(EdgeCollection)).call
.apply(_ref2, [this].concat(args)));

  _this6.type = types.EDGE_COLLECTION;
  return _this6;
}
```
- example usage
```shell
...
  key: 'collection',
  value: function collection(collectionName) {
    return new _collection.DocumentCollection(this._connection, collectionName);
  }
}, {
  key: 'edgeCollection',
  value: function edgeCollection(collectionName) {
    return new _collection.EdgeCollection(this._connection, collectionName);
  }
}, {
  key: 'listCollections',
  value: function listCollections(excludeSystem, cb) {
    if (typeof excludeSystem === 'function') {
      cb = excludeSystem;
      excludeSystem = undefined;
...
```

#### <a name="apidoc.element.arangojs.collection._BaseCollection"></a>[function <span class="apidocSignatureSpan">arangojs.collection.</span>_BaseCollection (connection, name)](#apidoc.element.arangojs.collection._BaseCollection)
- description and source-code
```javascript
function BaseCollection(connection, name) {
  _classCallCheck(this, BaseCollection);

  this.name = name;
  this._urlPrefix = '/collection/' + name + '/';
  this._idPrefix = name + '/';
  this._connection = connection;
  this._api = this._connection.route('/_api');
  if (this._connection.arangoMajor >= 3) {
    this.first = undefined;
    this.last = undefined;
    this.createCapConstraint = undefined;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.arangojs.collection.default"></a>[function <span class="apidocSignatureSpan">arangojs.collection.</span>default (connection, body)](#apidoc.element.arangojs.collection.default)
- description and source-code
```javascript
function construct(connection, body) {
  var Collection = body.type === types.EDGE_COLLECTION ? EdgeCollection : DocumentCollection;
  return new Collection(connection, body.name);
}
```
- example usage
```shell
...
    }

    var _connection$promisify12 = this._connection.promisify(cb),
        promise = _connection$promisify12.promise,
        callback = _connection$promisify12.callback;

    this._api.put('/simple/all', _extends({}, opts, { collection: this.name }), function (err, res) {
      return err ? callback(err) : callback(null, new _cursor2.default(_this2._connection, res.body));
    });
    return promise;
  }
}, {
  key: 'any',
  value: function any(cb) {
    var _connection$promisify13 = this._connection.promisify(cb),
...
```



# <a name="apidoc.module.arangojs.connection"></a>[module arangojs.connection](#apidoc.module.arangojs.connection)

#### <a name="apidoc.element.arangojs.connection.default"></a>[function <span class="apidocSignatureSpan">arangojs.connection.</span>default (config)](#apidoc.element.arangojs.connection.default)
- description and source-code
```javascript
function Connection(config) {
  _classCallCheck(this, Connection);

  if (typeof config === 'string') {
    config = { url: config };
  }
  this.config = _extends({}, Connection.defaults, config);
  this.config.agentOptions = _extends({}, Connection.agentDefaults, this.config.agentOptions);
  if (!this.config.headers) this.config.headers = {};
  if (!this.config.headers['x-arango-version']) {
    this.config.headers['x-arango-version'] = this.config.arangoVersion;
  }
  this.arangoMajor = Math.floor(this.config.arangoVersion / 10000);

  var _createRequest = (0, _request2.default)(this.config.url, this.config.agentOptions, this.config.agent),
      request = _createRequest.request,
      auth = _createRequest.auth,
      url = _createRequest.url;

  this._baseUrl = url;
  this._request = request;
  if (auth && !this.config.headers['authorization']) {
    this.config.headers['authorization'] = 'Basic ' + (0, _btoa2.default)(auth);
  }
  if (this.config.databaseName === false) {
    this._databasePath = '';
  } else {
    this._databasePath = '/_db/' + this.config.databaseName;
  }
  this.promisify = (0, _promisify3.default)(this.config.promise);
  this.retryOptions = {
    forever: this.config.retryConnection,
    retries: 0,
    minTimeout: 5000,
    randomize: true
  };
}
```
- example usage
```shell
...
    }

    var _connection$promisify12 = this._connection.promisify(cb),
        promise = _connection$promisify12.promise,
        callback = _connection$promisify12.callback;

    this._api.put('/simple/all', _extends({}, opts, { collection: this.name }), function (err, res) {
      return err ? callback(err) : callback(null, new _cursor2.default(_this2._connection, res.body));
    });
    return promise;
  }
}, {
  key: 'any',
  value: function any(cb) {
    var _connection$promisify13 = this._connection.promisify(cb),
...
```



# <a name="apidoc.module.arangojs.cursor"></a>[module arangojs.cursor](#apidoc.module.arangojs.cursor)

#### <a name="apidoc.element.arangojs.cursor.default"></a>[function <span class="apidocSignatureSpan">arangojs.cursor.</span>default (connection, body)](#apidoc.element.arangojs.cursor.default)
- description and source-code
```javascript
function ArrayCursor(connection, body) {
  _classCallCheck(this, ArrayCursor);

  this.extra = body.extra;
  this._connection = connection;
  this._api = this._connection.route('/_api');
  this._result = body.result;
  this._hasMore = Boolean(body.hasMore);
  this._id = body.id;
  this.count = body.count;
}
```
- example usage
```shell
...
    }

    var _connection$promisify12 = this._connection.promisify(cb),
        promise = _connection$promisify12.promise,
        callback = _connection$promisify12.callback;

    this._api.put('/simple/all', _extends({}, opts, { collection: this.name }), function (err, res) {
      return err ? callback(err) : callback(null, new _cursor2.default(_this2._connection, res.body));
    });
    return promise;
  }
}, {
  key: 'any',
  value: function any(cb) {
    var _connection$promisify13 = this._connection.promisify(cb),
...
```



# <a name="apidoc.module.arangojs.database"></a>[module arangojs.database](#apidoc.module.arangojs.database)

#### <a name="apidoc.element.arangojs.database.default"></a>[function <span class="apidocSignatureSpan">arangojs.database.</span>default (config)](#apidoc.element.arangojs.database.default)
- description and source-code
```javascript
function Database(config) {
  _classCallCheck(this, Database);

  this._connection = new _connection2.default(config);
  this._api = this._connection.route('/_api');
  this.name = this._connection.config.databaseName;
}
```
- example usage
```shell
...
    }

    var _connection$promisify12 = this._connection.promisify(cb),
        promise = _connection$promisify12.promise,
        callback = _connection$promisify12.callback;

    this._api.put('/simple/all', _extends({}, opts, { collection: this.name }), function (err, res) {
      return err ? callback(err) : callback(null, new _cursor2.default(_this2._connection, res.body));
    });
    return promise;
  }
}, {
  key: 'any',
  value: function any(cb) {
    var _connection$promisify13 = this._connection.promisify(cb),
...
```



# <a name="apidoc.module.arangojs.error"></a>[module arangojs.error](#apidoc.module.arangojs.error)

#### <a name="apidoc.element.arangojs.error.default"></a>[function <span class="apidocSignatureSpan">arangojs.error.</span>default (obj)](#apidoc.element.arangojs.error.default)
- description and source-code
```javascript
function ArangoError(obj) {
  _classCallCheck(this, ArangoError);

  var _this = _possibleConstructorReturn(this, (ArangoError.__proto__ || Object.getPrototypeOf(ArangoError)).call(this));

  _this.message = obj.errorMessage;
  _this.errorNum = obj.errorNum;
  _this.code = obj.code;
  var err = new Error(_this.message);
  err.name = _this.name;
  if (err.fileName) _this.fileName = err.fileName;
  if (err.lineNumber) _this.lineNumber = err.lineNumber;
  if (err.columnNumber) _this.columnNumber = err.columnNumber;
  if (err.stack) _this.stack = err.stack;
  if (err.description) _this.description = err.description;
  if (err.number) _this.number = err.number;
  return _this;
}
```
- example usage
```shell
...
    }

    var _connection$promisify12 = this._connection.promisify(cb),
        promise = _connection$promisify12.promise,
        callback = _connection$promisify12.callback;

    this._api.put('/simple/all', _extends({}, opts, { collection: this.name }), function (err, res) {
      return err ? callback(err) : callback(null, new _cursor2.default(_this2._connection, res.body));
    });
    return promise;
  }
}, {
  key: 'any',
  value: function any(cb) {
    var _connection$promisify13 = this._connection.promisify(cb),
...
```



# <a name="apidoc.module.arangojs.graph"></a>[module arangojs.graph](#apidoc.module.arangojs.graph)

#### <a name="apidoc.element.arangojs.graph.EdgeCollection"></a>[function <span class="apidocSignatureSpan">arangojs.graph.</span>EdgeCollection (connection, name, graph)](#apidoc.element.arangojs.graph.EdgeCollection)
- description and source-code
```javascript
function GraphEdgeCollection(connection, name, graph) {
  _classCallCheck(this, GraphEdgeCollection);

  var _this2 = _possibleConstructorReturn(this, (GraphEdgeCollection.__proto__ || Object.getPrototypeOf(GraphEdgeCollection)).call
(this, connection, name));

  _this2.type = _collection._types.EDGE_COLLECTION;
  _this2.graph = graph;
  _this2._gharial = _this2._api.route('/gharial/' + _this2.graph.name + '/edge');
  return _this2;
}
```
- example usage
```shell
...
  key: 'collection',
  value: function collection(collectionName) {
    return new _collection.DocumentCollection(this._connection, collectionName);
  }
}, {
  key: 'edgeCollection',
  value: function edgeCollection(collectionName) {
    return new _collection.EdgeCollection(this._connection, collectionName);
  }
}, {
  key: 'listCollections',
  value: function listCollections(excludeSystem, cb) {
    if (typeof excludeSystem === 'function') {
      cb = excludeSystem;
      excludeSystem = undefined;
...
```

#### <a name="apidoc.element.arangojs.graph.VertexCollection"></a>[function <span class="apidocSignatureSpan">arangojs.graph.</span>VertexCollection (connection, name, graph)](#apidoc.element.arangojs.graph.VertexCollection)
- description and source-code
```javascript
function GraphVertexCollection(connection, name, graph) {
  _classCallCheck(this, GraphVertexCollection);

  var _this = _possibleConstructorReturn(this, (GraphVertexCollection.__proto__ || Object.getPrototypeOf(GraphVertexCollection)).
call(this, connection, name));

  _this.type = _collection._types.DOCUMENT_COLLECTION;
  _this.graph = graph;
  _this._gharial = _this._api.route('/gharial/' + _this.graph.name + '/vertex');
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.arangojs.graph.default"></a>[function <span class="apidocSignatureSpan">arangojs.graph.</span>default (connection, name)](#apidoc.element.arangojs.graph.default)
- description and source-code
```javascript
function Graph(connection, name) {
  _classCallCheck(this, Graph);

  this.name = name;
  this._connection = connection;
  this._api = this._connection.route('/_api');
  this._gharial = this._api.route('/gharial/' + this.name);
}
```
- example usage
```shell
...
    }

    var _connection$promisify12 = this._connection.promisify(cb),
        promise = _connection$promisify12.promise,
        callback = _connection$promisify12.callback;

    this._api.put('/simple/all', _extends({}, opts, { collection: this.name }), function (err, res) {
      return err ? callback(err) : callback(null, new _cursor2.default(_this2._connection, res.body));
    });
    return promise;
  }
}, {
  key: 'any',
  value: function any(cb) {
    var _connection$promisify13 = this._connection.promisify(cb),
...
```



# <a name="apidoc.module.arangojs.route"></a>[module arangojs.route](#apidoc.module.arangojs.route)

#### <a name="apidoc.element.arangojs.route.default"></a>[function <span class="apidocSignatureSpan">arangojs.route.</span>default (connection, path, headers)](#apidoc.element.arangojs.route.default)
- description and source-code
```javascript
function Route(connection, path, headers) {
  _classCallCheck(this, Route);

  if (!path) path = '';else if (path.charAt(0) !== '/') path = '/' + path;
  this._connection = connection;
  this._path = path;
  this._headers = headers;
}
```
- example usage
```shell
...
    }

    var _connection$promisify12 = this._connection.promisify(cb),
        promise = _connection$promisify12.promise,
        callback = _connection$promisify12.callback;

    this._api.put('/simple/all', _extends({}, opts, { collection: this.name }), function (err, res) {
      return err ? callback(err) : callback(null, new _cursor2.default(_this2._connection, res.body));
    });
    return promise;
  }
}, {
  key: 'any',
  value: function any(cb) {
    var _connection$promisify13 = this._connection.promisify(cb),
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
