# api documentation for  [js2xmlparser (v3.0.0)](https://github.com/michaelkourlas/node-js2xmlparser#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-js2xmlparser.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-js2xmlparser) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-js2xmlparser.svg)](https://travis-ci.org/npmdoc/node-npmdoc-js2xmlparser)
#### Parses JavaScript objects into XML

[![NPM](https://nodei.co/npm/js2xmlparser.png?downloads=true)](https://www.npmjs.com/package/js2xmlparser)

[![apidoc](https://npmdoc.github.io/node-npmdoc-js2xmlparser/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-js2xmlparser_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-js2xmlparser/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-js2xmlparser/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-js2xmlparser/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Michael Kourlas",
        "email": "michael@kourlas.net"
    },
    "bugs": {
        "url": "https://github.com/michaelkourlas/node-js2xmlparser/issues"
    },
    "dependencies": {
        "xmlcreate": "^1.0.1"
    },
    "description": "Parses JavaScript objects into XML",
    "devDependencies": {
        "@types/chai": "^3.4.35",
        "@types/mocha": "^2.2.39",
        "chai": "^3.5.0",
        "del": "^2.2.2",
        "gulp": "^3.9.1",
        "gulp-mocha": "^4.0.1",
        "gulp-sourcemaps": "^2.4.1",
        "gulp-tslint": "^7.1.0",
        "gulp-typedoc": "^2.0.2",
        "gulp-typescript": "^3.1.5",
        "merge2": "^1.0.3",
        "mocha": "^3.2.0",
        "tslint": "^4.4.2",
        "typedoc": "^0.5.7",
        "typescript": "^2.1.6"
    },
    "directories": {},
    "dist": {
        "shasum": "3fb60eaa089c5440f9319f51760ccd07e2499733",
        "tarball": "https://registry.npmjs.org/js2xmlparser/-/js2xmlparser-3.0.0.tgz"
    },
    "files": [
        "lib",
        "CHANGES.md",
        "LICENSE.md",
        "NOTICE.md",
        "package.json",
        "README.md"
    ],
    "gitHead": "debf3ad08ca3f8795e0498a2a84a4390d0f6fc50",
    "homepage": "https://github.com/michaelkourlas/node-js2xmlparser#readme",
    "keywords": [
        "convert",
        "converter",
        "javascript",
        "js",
        "json",
        "object",
        "objects",
        "parse",
        "parser",
        "xml"
    ],
    "license": "Apache-2.0",
    "main": "./lib/main.js",
    "maintainers": [
        {
            "name": "michaelkourlas",
            "email": "michaelkourlas@gmail.com"
        }
    ],
    "name": "js2xmlparser",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/michaelkourlas/node-js2xmlparser.git"
    },
    "scripts": {},
    "typings": "./lib/main",
    "version": "3.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module js2xmlparser](#apidoc.module.js2xmlparser)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.</span>parse (root, object, options)](#apidoc.element.js2xmlparser.parse)
1.  object <span class="apidocSignatureSpan">js2xmlparser.</span>options
1.  object <span class="apidocSignatureSpan">js2xmlparser.</span>utils

#### [module js2xmlparser.options](#apidoc.module.js2xmlparser.options)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.options.</span>DeclarationOptions (declarationOptions)](#apidoc.element.js2xmlparser.options.DeclarationOptions)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.options.</span>DtdOptions (dtdOptions)](#apidoc.element.js2xmlparser.options.DtdOptions)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.options.</span>FormatOptions (formatOptions)](#apidoc.element.js2xmlparser.options.FormatOptions)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.options.</span>Options (options)](#apidoc.element.js2xmlparser.options.Options)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.options.</span>TypeHandlers (typeHandlers)](#apidoc.element.js2xmlparser.options.TypeHandlers)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.options.</span>WrapHandlers (wrapHandlers)](#apidoc.element.js2xmlparser.options.WrapHandlers)

#### [module js2xmlparser.utils](#apidoc.module.js2xmlparser.utils)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isArray (val)](#apidoc.element.js2xmlparser.utils.isArray)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isBoolean (val)](#apidoc.element.js2xmlparser.utils.isBoolean)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isFunction (val)](#apidoc.element.js2xmlparser.utils.isFunction)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isMap (val)](#apidoc.element.js2xmlparser.utils.isMap)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isNull (val)](#apidoc.element.js2xmlparser.utils.isNull)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isNumber (val)](#apidoc.element.js2xmlparser.utils.isNumber)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isObject (val)](#apidoc.element.js2xmlparser.utils.isObject)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isPrimitive (val)](#apidoc.element.js2xmlparser.utils.isPrimitive)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isSet (val)](#apidoc.element.js2xmlparser.utils.isSet)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isString (val)](#apidoc.element.js2xmlparser.utils.isString)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isStringArray (val)](#apidoc.element.js2xmlparser.utils.isStringArray)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isUndefined (val)](#apidoc.element.js2xmlparser.utils.isUndefined)
1.  [function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>stringify (value)](#apidoc.element.js2xmlparser.utils.stringify)



# <a name="apidoc.module.js2xmlparser"></a>[module js2xmlparser](#apidoc.module.js2xmlparser)

#### <a name="apidoc.element.js2xmlparser.parse"></a>[function <span class="apidocSignatureSpan">js2xmlparser.</span>parse (root, object, options)](#apidoc.element.js2xmlparser.parse)
- description and source-code
```javascript
function parse(root, object, options) {
    var opts = new options_1.Options(options);
    var document = parseToDocument(root, object, opts);
    return document.toString(opts.format);
}
```
- example usage
```shell
...
            },
            "#": "567-555-8901"
        }
    ],
    "email": "john@smith.com"
};

console.log(js2xmlparser.parse("person", obj));
'''

This example produces the following XML:

'''xml
<?xml version='1.0'?>
<person>
...
```



# <a name="apidoc.module.js2xmlparser.options"></a>[module js2xmlparser.options](#apidoc.module.js2xmlparser.options)

#### <a name="apidoc.element.js2xmlparser.options.DeclarationOptions"></a>[function <span class="apidocSignatureSpan">js2xmlparser.options.</span>DeclarationOptions (declarationOptions)](#apidoc.element.js2xmlparser.options.DeclarationOptions)
- description and source-code
```javascript
function DeclarationOptions(declarationOptions) {
    if (declarationOptions === void 0) { declarationOptions = {}; }
    this.include = true;
    if (!utils_1.isObject(declarationOptions)) {
        throw new TypeError("options.declaration should be an Object or"
            + " undefined");
    }
    if (!utils_1.isBoolean(declarationOptions.include)) {
        if (!utils_1.isUndefined(declarationOptions.include)) {
            throw new TypeError("options.declaration.include should be a"
                + " boolean or undefined");
        }
    }
    else {
        this.include = declarationOptions.include;
    }
    // Validation performed by xmlcreate
    this.encoding = declarationOptions.encoding;
    this.standalone = declarationOptions.standalone;
    this.version = declarationOptions.version;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js2xmlparser.options.DtdOptions"></a>[function <span class="apidocSignatureSpan">js2xmlparser.options.</span>DtdOptions (dtdOptions)](#apidoc.element.js2xmlparser.options.DtdOptions)
- description and source-code
```javascript
function DtdOptions(dtdOptions) {
    if (dtdOptions === void 0) { dtdOptions = {}; }
    this.include = false;
    if (!utils_1.isObject(dtdOptions)) {
        throw new TypeError("options.dtd should be an Object or undefined");
    }
    if (!utils_1.isBoolean(dtdOptions.include)) {
        if (!utils_1.isUndefined(dtdOptions.include)) {
            throw new TypeError("options.dtd.include should be a boolean"
                + " or undefined");
        }
    }
    else {
        this.include = dtdOptions.include;
    }
    // Validation performed by xmlcreate
    this.name = dtdOptions.name;
    this.sysId = dtdOptions.sysId;
    this.pubId = dtdOptions.pubId;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js2xmlparser.options.FormatOptions"></a>[function <span class="apidocSignatureSpan">js2xmlparser.options.</span>FormatOptions (formatOptions)](#apidoc.element.js2xmlparser.options.FormatOptions)
- description and source-code
```javascript
function FormatOptions(formatOptions) {
    if (formatOptions === void 0) { formatOptions = {}; }
    if (!utils_1.isObject(formatOptions)) {
        throw new TypeError("options.format should be an Object or"
            + " undefined");
    }
    // Validation performed by xmlcreate
    this.doubleQuotes = formatOptions.doubleQuotes;
    this.indent = formatOptions.indent;
    this.newline = formatOptions.newline;
    this.pretty = formatOptions.pretty;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js2xmlparser.options.Options"></a>[function <span class="apidocSignatureSpan">js2xmlparser.options.</span>Options (options)](#apidoc.element.js2xmlparser.options.Options)
- description and source-code
```javascript
function Options(options) {
    if (options === void 0) { options = {}; }
    this.aliasString = "=";
    this.attributeString = "@";
    this.cdataInvalidChars = false;
    this.cdataKeys = [];
    this.valueString = "#";
    if (!utils_1.isObject(options)) {
        throw new TypeError("options should be an Object or undefined");
    }
    if (!utils_1.isString(options.aliasString)) {
        if (!utils_1.isUndefined(options.aliasString)) {
            throw new TypeError("options.aliasString should be a string or"
                + " undefined");
        }
    }
    else {
        this.aliasString = options.aliasString;
    }
    if (!utils_1.isString(options.attributeString)) {
        if (!utils_1.isUndefined(options.attributeString)) {
            throw new TypeError("options.attributeString should be a string"
                + " or undefined");
        }
    }
    else {
        this.attributeString = options.attributeString;
    }
    if (!utils_1.isBoolean(options.cdataInvalidChars)) {
        if (!utils_1.isUndefined(options.cdataInvalidChars)) {
            throw new TypeError("options.cdataInvalidChars should be a"
                + " boolean or undefined");
        }
    }
    else {
        this.cdataInvalidChars = options.cdataInvalidChars;
    }
    if (!utils_1.isStringArray(options.cdataKeys)) {
        if (!utils_1.isUndefined(options.cdataKeys)) {
            throw new TypeError("options.cdataKeys should be an Array or" +
                " undefined");
        }
    }
    else {
        this.cdataKeys = options.cdataKeys;
    }
    this.declaration = new DeclarationOptions(options.declaration);
    this.dtd = new DtdOptions(options.dtd);
    this.format = new FormatOptions(options.format);
    this.typeHandlers = new TypeHandlers(options.typeHandlers);
    if (!utils_1.isString(options.valueString)) {
        if (!utils_1.isUndefined(options.valueString)) {
            throw new TypeError("options.valueString should be a string"
                + " or undefined");
        }
    }
    else {
        this.valueString = options.valueString;
    }
    this.wrapHandlers = new WrapHandlers(options.wrapHandlers);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js2xmlparser.options.TypeHandlers"></a>[function <span class="apidocSignatureSpan">js2xmlparser.options.</span>TypeHandlers (typeHandlers)](#apidoc.element.js2xmlparser.options.TypeHandlers)
- description and source-code
```javascript
function TypeHandlers(typeHandlers) {
    if (typeHandlers === void 0) { typeHandlers = {}; }
    if (!utils_1.isObject(typeHandlers)) {
        throw new TypeError("options.typeHandlers should be an Object or"
            + " undefined");
    }
    for (var key in typeHandlers) {
        if (typeHandlers.hasOwnProperty(key)) {
            if (!utils_1.isFunction(typeHandlers[key])) {
                throw new TypeError("options.typeHandlers['" + key + "']" +
                    " should be a Function");
            }
            else {
                this[key] = typeHandlers[key];
            }
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js2xmlparser.options.WrapHandlers"></a>[function <span class="apidocSignatureSpan">js2xmlparser.options.</span>WrapHandlers (wrapHandlers)](#apidoc.element.js2xmlparser.options.WrapHandlers)
- description and source-code
```javascript
function WrapHandlers(wrapHandlers) {
    if (wrapHandlers === void 0) { wrapHandlers = {}; }
    if (!utils_1.isObject(wrapHandlers)) {
        throw new TypeError("options.wrapHandlers should be an Object or"
            + " undefined");
    }
    for (var key in wrapHandlers) {
        if (wrapHandlers.hasOwnProperty(key)) {
            if (!utils_1.isFunction(wrapHandlers[key])) {
                throw new TypeError("options.wrapHandlers['" + key + "']" +
                    " should be a Function");
            }
            else {
                this[key] = wrapHandlers[key];
            }
        }
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.js2xmlparser.utils"></a>[module js2xmlparser.utils](#apidoc.module.js2xmlparser.utils)

#### <a name="apidoc.element.js2xmlparser.utils.isArray"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isArray (val)](#apidoc.element.js2xmlparser.utils.isArray)
- description and source-code
```javascript
function isArray(val) {
    return Object.prototype.toString.call(val) === "[object Array]";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js2xmlparser.utils.isBoolean"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isBoolean (val)](#apidoc.element.js2xmlparser.utils.isBoolean)
- description and source-code
```javascript
function isBoolean(val) {
    return Object.prototype.toString.call(val) === "[object Boolean]";
}
```
- example usage
```shell
...
        throw new TypeError("options.attributeString should be a string"
            + " or undefined");
    }
}
else {
    this.attributeString = options.attributeString;
}
if (!utils_1.isBoolean(options.cdataInvalidChars)) {
    if (!utils_1.isUndefined(options.cdataInvalidChars)) {
        throw new TypeError("options.cdataInvalidChars should be a"
            + " boolean or undefined");
    }
}
else {
    this.cdataInvalidChars = options.cdataInvalidChars;
...
```

#### <a name="apidoc.element.js2xmlparser.utils.isFunction"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isFunction (val)](#apidoc.element.js2xmlparser.utils.isFunction)
- description and source-code
```javascript
function isFunction(val) {
    return Object.prototype.toString.call(val) === "[object Function]";
}
```
- example usage
```shell
...
if (typeHandlers === void 0) { typeHandlers = {}; }
if (!utils_1.isObject(typeHandlers)) {
    throw new TypeError("options.typeHandlers should be an Object or"
        + " undefined");
}
for (var key in typeHandlers) {
    if (typeHandlers.hasOwnProperty(key)) {
        if (!utils_1.isFunction(typeHandlers[key])) {
            throw new TypeError("options.typeHandlers['" + key + "']" +
                " should be a Function");
        }
        else {
            this[key] = typeHandlers[key];
        }
    }
...
```

#### <a name="apidoc.element.js2xmlparser.utils.isMap"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isMap (val)](#apidoc.element.js2xmlparser.utils.isMap)
- description and source-code
```javascript
function isMap(val) {
    return Object.prototype.toString.call(val) === "[object Map]";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js2xmlparser.utils.isNull"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isNull (val)](#apidoc.element.js2xmlparser.utils.isNull)
- description and source-code
```javascript
function isNull(val) {
    return Object.prototype.toString.call(val) === "[object Null]";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js2xmlparser.utils.isNumber"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isNumber (val)](#apidoc.element.js2xmlparser.utils.isNumber)
- description and source-code
```javascript
function isNumber(val) {
    return Object.prototype.toString.call(val) === "[object Number]";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js2xmlparser.utils.isObject"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isObject (val)](#apidoc.element.js2xmlparser.utils.isObject)
- description and source-code
```javascript
function isObject(val) {
    return Object.prototype.toString.call(val) === "[object Object]";
}
```
- example usage
```shell
...
    function Options(options) {
if (options === void 0) { options = {}; }
this.aliasString = "=";
this.attributeString = "@";
this.cdataInvalidChars = false;
this.cdataKeys = [];
this.valueString = "#";
if (!utils_1.isObject(options)) {
    throw new TypeError("options should be an Object or undefined");
}
if (!utils_1.isString(options.aliasString)) {
    if (!utils_1.isUndefined(options.aliasString)) {
        throw new TypeError("options.aliasString should be a string or"
            + " undefined");
    }
...
```

#### <a name="apidoc.element.js2xmlparser.utils.isPrimitive"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isPrimitive (val)](#apidoc.element.js2xmlparser.utils.isPrimitive)
- description and source-code
```javascript
function isPrimitive(val) {
    return isString(val)
        || isNumber(val)
        || isBoolean(val)
        || isUndefined(val)
        || isNull(val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js2xmlparser.utils.isSet"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isSet (val)](#apidoc.element.js2xmlparser.utils.isSet)
- description and source-code
```javascript
function isSet(val) {
    return Object.prototype.toString.call(val) === "[object Set]";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js2xmlparser.utils.isString"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isString (val)](#apidoc.element.js2xmlparser.utils.isString)
- description and source-code
```javascript
function isString(val) {
    return Object.prototype.toString.call(val) === "[object String]";
}
```
- example usage
```shell
...
this.attributeString = "@";
this.cdataInvalidChars = false;
this.cdataKeys = [];
this.valueString = "#";
if (!utils_1.isObject(options)) {
    throw new TypeError("options should be an Object or undefined");
}
if (!utils_1.isString(options.aliasString)) {
    if (!utils_1.isUndefined(options.aliasString)) {
        throw new TypeError("options.aliasString should be a string or"
            + " undefined");
    }
}
else {
    this.aliasString = options.aliasString;
...
```

#### <a name="apidoc.element.js2xmlparser.utils.isStringArray"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isStringArray (val)](#apidoc.element.js2xmlparser.utils.isStringArray)
- description and source-code
```javascript
function isStringArray(val) {
    if (!isArray(val)) {
        return false;
    }
    for (var _i = 0, val_1 = val; _i < val_1.length; _i++) {
        var entry = val_1[_i];
        if (!isString(entry)) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
        throw new TypeError("options.cdataInvalidChars should be a"
            + " boolean or undefined");
    }
}
else {
    this.cdataInvalidChars = options.cdataInvalidChars;
}
if (!utils_1.isStringArray(options.cdataKeys)) {
    if (!utils_1.isUndefined(options.cdataKeys)) {
        throw new TypeError("options.cdataKeys should be an Array or" +
            " undefined");
    }
}
else {
    this.cdataKeys = options.cdataKeys;
...
```

#### <a name="apidoc.element.js2xmlparser.utils.isUndefined"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>isUndefined (val)](#apidoc.element.js2xmlparser.utils.isUndefined)
- description and source-code
```javascript
function isUndefined(val) {
    return Object.prototype.toString.call(val) === "[object Undefined]";
}
```
- example usage
```shell
...
this.cdataInvalidChars = false;
this.cdataKeys = [];
this.valueString = "#";
if (!utils_1.isObject(options)) {
    throw new TypeError("options should be an Object or undefined");
}
if (!utils_1.isString(options.aliasString)) {
    if (!utils_1.isUndefined(options.aliasString)) {
        throw new TypeError("options.aliasString should be a string or"
            + " undefined");
    }
}
else {
    this.aliasString = options.aliasString;
}
...
```

#### <a name="apidoc.element.js2xmlparser.utils.stringify"></a>[function <span class="apidocSignatureSpan">js2xmlparser.utils.</span>stringify (value)](#apidoc.element.js2xmlparser.utils.stringify)
- description and source-code
```javascript
function stringify(value) {
    if (!isUndefined(value) && !isNull(value)) {
        if (!isFunction(value.toString)) {
            value = value.toString();
        }
    }
    return String(value);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
