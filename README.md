# api documentation for  [cheerio (v0.22.0)](https://github.com/cheeriojs/cheerio#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-cheerio.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cheerio) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cheerio.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cheerio)
#### Tiny, fast, and elegant implementation of core jQuery designed specifically for the server

[![NPM](https://nodei.co/npm/cheerio.png?downloads=true)](https://www.npmjs.com/package/cheerio)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cheerio/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-cheerio_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cheerio/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cheerio/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cheerio/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matt Mueller",
        "email": "mattmuelle@gmail.com",
        "url": "mat.io"
    },
    "bugs": {
        "url": "https://github.com/cheeriojs/cheerio/issues"
    },
    "dependencies": {
        "css-select": "~1.2.0",
        "dom-serializer": "~0.1.0",
        "entities": "~1.1.1",
        "htmlparser2": "^3.9.1",
        "lodash.assignin": "^4.0.9",
        "lodash.bind": "^4.1.4",
        "lodash.defaults": "^4.0.1",
        "lodash.filter": "^4.4.0",
        "lodash.flatten": "^4.2.0",
        "lodash.foreach": "^4.3.0",
        "lodash.map": "^4.4.0",
        "lodash.merge": "^4.4.0",
        "lodash.pick": "^4.2.1",
        "lodash.reduce": "^4.4.0",
        "lodash.reject": "^4.4.0",
        "lodash.some": "^4.4.0"
    },
    "description": "Tiny, fast, and elegant implementation of core jQuery designed specifically for the server",
    "devDependencies": {
        "benchmark": "^2.1.0",
        "coveralls": "^2.11.9",
        "expect.js": "~0.3.1",
        "istanbul": "^0.4.3",
        "jquery": "^3.0.0",
        "jsdom": "^9.2.1",
        "jshint": "^2.9.2",
        "mocha": "^2.5.3",
        "xyz": "~0.5.0"
    },
    "directories": {},
    "dist": {
        "shasum": "a9baa860a3f9b595a6b81b1a86873121ed3a269e",
        "tarball": "https://registry.npmjs.org/cheerio/-/cheerio-0.22.0.tgz"
    },
    "engines": {
        "node": ">= 0.6"
    },
    "files": [
        "index.js",
        "lib"
    ],
    "gitHead": "35c4917205dca9d08139c95419e2626c0689e38a",
    "homepage": "https://github.com/cheeriojs/cheerio#readme",
    "keywords": [
        "htmlparser",
        "jquery",
        "selector",
        "scraper",
        "parser",
        "html"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "mattmueller",
            "email": "mattmuelle@gmail.com"
        },
        {
            "name": "davidchambers",
            "email": "dc@davidchambers.me"
        },
        {
            "name": "jugglinmike",
            "email": "mike@mikepennisi.com"
        },
        {
            "name": "feedic",
            "email": "me@feedic.com"
        }
    ],
    "name": "cheerio",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/cheeriojs/cheerio.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "0.22.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module cheerio](#apidoc.module.cheerio)
1.  [function <span class="apidocSignatureSpan">cheerio.</span>contains (container, contained)](#apidoc.element.cheerio.contains)
1.  [function <span class="apidocSignatureSpan">cheerio.</span>html (dom, options)](#apidoc.element.cheerio.html)
1.  [function <span class="apidocSignatureSpan">cheerio.</span>load (content, options)](#apidoc.element.cheerio.load)
1.  [function <span class="apidocSignatureSpan">cheerio.</span>parse (content, options)](#apidoc.element.cheerio.parse)
1.  [function <span class="apidocSignatureSpan">cheerio.</span>parseHTML (data, context, keepScripts)](#apidoc.element.cheerio.parseHTML)
1.  [function <span class="apidocSignatureSpan">cheerio.</span>root ()](#apidoc.element.cheerio.root)
1.  [function <span class="apidocSignatureSpan">cheerio.</span>text (elems)](#apidoc.element.cheerio.text)
1.  [function <span class="apidocSignatureSpan">cheerio.</span>xml (dom)](#apidoc.element.cheerio.xml)
1.  object <span class="apidocSignatureSpan">cheerio.</span>static
1.  object <span class="apidocSignatureSpan">cheerio.</span>utils
1.  string <span class="apidocSignatureSpan">cheerio.</span>version

#### [module cheerio.parse](#apidoc.module.cheerio.parse)
1.  [function <span class="apidocSignatureSpan">cheerio.</span>parse (content, options)](#apidoc.element.cheerio.parse.parse)
1.  [function <span class="apidocSignatureSpan">cheerio.parse.</span>evaluate (content, options)](#apidoc.element.cheerio.parse.evaluate)
1.  [function <span class="apidocSignatureSpan">cheerio.parse.</span>update (arr, parent)](#apidoc.element.cheerio.parse.update)

#### [module cheerio.static](#apidoc.module.cheerio.static)
1.  [function <span class="apidocSignatureSpan">cheerio.static.</span>contains (container, contained)](#apidoc.element.cheerio.static.contains)
1.  [function <span class="apidocSignatureSpan">cheerio.static.</span>html (dom, options)](#apidoc.element.cheerio.static.html)
1.  [function <span class="apidocSignatureSpan">cheerio.static.</span>load (content, options)](#apidoc.element.cheerio.static.load)
1.  [function <span class="apidocSignatureSpan">cheerio.static.</span>parseHTML (data, context, keepScripts)](#apidoc.element.cheerio.static.parseHTML)
1.  [function <span class="apidocSignatureSpan">cheerio.static.</span>root ()](#apidoc.element.cheerio.static.root)
1.  [function <span class="apidocSignatureSpan">cheerio.static.</span>text (elems)](#apidoc.element.cheerio.static.text)
1.  [function <span class="apidocSignatureSpan">cheerio.static.</span>xml (dom)](#apidoc.element.cheerio.static.xml)

#### [module cheerio.utils](#apidoc.module.cheerio.utils)
1.  [function <span class="apidocSignatureSpan">cheerio.utils.</span>camelCase (str)](#apidoc.element.cheerio.utils.camelCase)
1.  [function <span class="apidocSignatureSpan">cheerio.utils.</span>cloneDom (dom, options)](#apidoc.element.cheerio.utils.cloneDom)
1.  [function <span class="apidocSignatureSpan">cheerio.utils.</span>cssCase (str)](#apidoc.element.cheerio.utils.cssCase)
1.  [function <span class="apidocSignatureSpan">cheerio.utils.</span>domEach (cheerio, fn)](#apidoc.element.cheerio.utils.domEach)
1.  [function <span class="apidocSignatureSpan">cheerio.utils.</span>isHtml (str)](#apidoc.element.cheerio.utils.isHtml)
1.  [function <span class="apidocSignatureSpan">cheerio.utils.</span>isTag (type)](#apidoc.element.cheerio.utils.isTag)



# <a name="apidoc.module.cheerio"></a>[module cheerio](#apidoc.module.cheerio)

#### <a name="apidoc.element.cheerio.contains"></a>[function <span class="apidocSignatureSpan">cheerio.</span>contains (container, contained)](#apidoc.element.cheerio.contains)
- description and source-code
```javascript
contains = function (container, contained) {

  // According to the jQuery API, an element does not "contain" itself
  if (contained === container) {
    return false;
  }

  // Step up the descendants, stopping when the root element is reached
  // (signaled by '.parent' returning a reference to the same object)
  while (contained && contained !== contained.parent) {
    contained = contained.parent;
    if (contained === container) {
      return true;
    }
  }

  return false;
}
```
- example usage
```shell
...
Sometimes you need to work with the top-level root element. To query it, you can use '$.root()'.

'''js
$.root().append('<ul id="vegetables"></ul>').html();
//=> <ul id="fruits">...</ul><ul id="vegetables"></ul>
'''

#### $.contains( container, contained )
Checks to see if the 'contained' DOM element is a descendant of the 'container' DOM element.

#### $.parseHTML( data [, context ] [, keepScripts ] )
Parses a string into an array of DOM nodes. The 'context' argument has no meaning for Cheerio, but it is maintained for API compatability
.

#### $.load( html[, options ] )
Load in the HTML. (See the previous section titled "Loading" for more information.)
...
```

#### <a name="apidoc.element.cheerio.html"></a>[function <span class="apidocSignatureSpan">cheerio.</span>html (dom, options)](#apidoc.element.cheerio.html)
- description and source-code
```javascript
html = function (dom, options) {
  var Cheerio = require('./cheerio');

  // be flexible about parameters, sometimes we call html(),
  // with options as only parameter
  // check dom argument for dom element specific properties
  // assume there is no 'length' or 'type' properties in the options object
  if (Object.prototype.toString.call(dom) === '[object Object]' && !options && !('length' in dom) && !('type' in dom))
  {
    options = dom;
    dom = undefined;
  }

  // sometimes $.html() used without preloading html
  // so fallback non existing options to the default ones
  options = _.defaults(options || {}, this._options, Cheerio.prototype.options);

  return render(this, dom, options);
}
```
- example usage
```shell
...
'''js
let cheerio = require('cheerio')
let $ = cheerio.load('<h2 class="title">Hello world</h2>')

$('h2.title').text('Hello there!')
$('h2').addClass('welcome')

$.html()
//=> <h2 class="title welcome">Hello there!</h2>
'''

## Installation
'npm install cheerio'

## Features
...
```

#### <a name="apidoc.element.cheerio.load"></a>[function <span class="apidocSignatureSpan">cheerio.</span>load (content, options)](#apidoc.element.cheerio.load)
- description and source-code
```javascript
load = function (content, options) {
  var Cheerio = require('./cheerio');

  options = _.defaults(options || {}, Cheerio.prototype.options);

  var root = parse(content, options);

  var initialize = function(selector, context, r, opts) {
    if (!(this instanceof initialize)) {
      return new initialize(selector, context, r, opts);
    }
    opts = _.defaults(opts || {}, options);
    return Cheerio.call(this, selector, context, r || root, opts);
  };

  // Ensure that selections created by the "loaded" 'initialize' function are
  // true Cheerio instances.
  initialize.prototype = Object.create(Cheerio.prototype);
  initialize.prototype.constructor = initialize;

  // Mimic jQuery's prototype alias for plugin authors.
  initialize.fn = initialize.prototype;

  // Keep a reference to the top-level scope so we can chain methods that implicitly
  // resolve selectors; e.g. $("<span>").(".bar"), which otherwise loses ._root
  initialize.prototype._originalRoot = root;

  // Add in the static methods
  _.merge(initialize, exports);

  // Add in the root
  initialize._root = root;
  // store options
  initialize._options = options;

  return initialize;
}
```
- example usage
```shell
...
  </a>
</div>

<br />

'''js
let cheerio = require('cheerio')
let $ = cheerio.load('<h2 class="title">Hello world</h2>')

$('h2.title').text('Hello there!')
$('h2').addClass('welcome')

$.html()
//=> <h2 class="title welcome">Hello there!</h2>
'''
...
```

#### <a name="apidoc.element.cheerio.parse"></a>[function <span class="apidocSignatureSpan">cheerio.</span>parse (content, options)](#apidoc.element.cheerio.parse)
- description and source-code
```javascript
parse = function (content, options) {
  var dom = exports.evaluate(content, options),
      // Generic root element
      root = exports.evaluate('<root></root>', options)[0];

  root.type = 'root';

  // Update the dom using the root
  exports.update(dom, root);

  return root;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cheerio.parseHTML"></a>[function <span class="apidocSignatureSpan">cheerio.</span>parseHTML (data, context, keepScripts)](#apidoc.element.cheerio.parseHTML)
- description and source-code
```javascript
parseHTML = function (data, context, keepScripts) {
  var parsed;

  if (!data || typeof data !== 'string') {
    return null;
  }

  if (typeof context === 'boolean') {
    keepScripts = context;
  }

  parsed = this.load(data);
  if (!keepScripts) {
    parsed('script').remove();
  }

  // The 'children' array is used by Cheerio internally to group elements that
  // share the same parents. When nodes created through 'parseHTML' are
  // inserted into previously-existing DOM structures, they will be removed
  // from the 'children' array. The results of 'parseHTML' should remain
  // constant across these operations, so a shallow copy should be returned.
  return parsed.root()[0].children.slice();
}
```
- example usage
```shell
...
$.root().append('<ul id="vegetables"></ul>').html();
//=> <ul id="fruits">...</ul><ul id="vegetables"></ul>
'''

#### $.contains( container, contained )
Checks to see if the 'contained' DOM element is a descendant of the 'container' DOM element.

#### $.parseHTML( data [, context ] [, keepScripts ] )
Parses a string into an array of DOM nodes. The 'context' argument has no meaning for Cheerio, but it is maintained for API compatability
.

#### $.load( html[, options ] )
Load in the HTML. (See the previous section titled "Loading" for more information.)

### Plugins
...
```

#### <a name="apidoc.element.cheerio.root"></a>[function <span class="apidocSignatureSpan">cheerio.</span>root ()](#apidoc.element.cheerio.root)
- description and source-code
```javascript
root = function () {
  return this(this._root);
}
```
- example usage
```shell
...
var moreFruit = $('#fruits').clone()
'''

### Utilities

#### $.root

Sometimes you need to work with the top-level root element. To query it, you can use '$.root()'.

'''js
$.root().append('<ul id="vegetables"></ul>').html();
//=> <ul id="fruits">...</ul><ul id="vegetables"></ul>
'''

#### $.contains( container, contained )
...
```

#### <a name="apidoc.element.cheerio.text"></a>[function <span class="apidocSignatureSpan">cheerio.</span>text (elems)](#apidoc.element.cheerio.text)
- description and source-code
```javascript
text = function (elems) {
  if (!elems) {
    elems = this.root();
  }

  var ret = '',
      len = elems.length,
      elem;

  for (var i = 0; i < len; i++) {
    elem = elems[i];
    if (elem.type === 'text') ret += elem.data;
    else if (elem.children && elem.type !== 'comment') {
      ret += exports.text(elem.children);
    }
  }

  return ret;
}
```
- example usage
```shell
...

<br />

'''js
let cheerio = require('cheerio')
let $ = cheerio.load('<h2 class="title">Hello world</h2>')

$('h2.title').text('Hello there!')
$('h2').addClass('welcome')

$.html()
//=> <h2 class="title welcome">Hello there!</h2>
'''

## Installation
...
```

#### <a name="apidoc.element.cheerio.xml"></a>[function <span class="apidocSignatureSpan">cheerio.</span>xml (dom)](#apidoc.element.cheerio.xml)
- description and source-code
```javascript
xml = function (dom) {
  var options = _.defaults({xmlMode: true}, this._options);

  return render(this, dom, options);
}
```
- example usage
```shell
...
'''xml
$ = cheerio.load('<media:thumbnail url="http://www.foo.com/keyframe.jpg" width="75" height="50" time="12:05:01.123"/>');
'''

... and later want to render to XML. To do this, you can use the 'xml' utility function:

'''js
$.xml()
//=>  <media:thumbnail url="http://www.foo.com/keyframe.jpg" width="75" height="50" time="12:05:01.123"/>
'''

You may also render the text content of a Cheerio object using the 'text' static method:

'''js
$ = cheerio.load('This is <em>content</em>.')
...
```



# <a name="apidoc.module.cheerio.parse"></a>[module cheerio.parse](#apidoc.module.cheerio.parse)

#### <a name="apidoc.element.cheerio.parse.parse"></a>[function <span class="apidocSignatureSpan">cheerio.</span>parse (content, options)](#apidoc.element.cheerio.parse.parse)
- description and source-code
```javascript
parse = function (content, options) {
  var dom = exports.evaluate(content, options),
      // Generic root element
      root = exports.evaluate('<root></root>', options)[0];

  root.type = 'root';

  // Update the dom using the root
  exports.update(dom, root);

  return root;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cheerio.parse.evaluate"></a>[function <span class="apidocSignatureSpan">cheerio.parse.</span>evaluate (content, options)](#apidoc.element.cheerio.parse.evaluate)
- description and source-code
```javascript
evaluate = function (content, options) {
  // options = options || $.fn.options;

  var dom;

  if (typeof content === 'string' || Buffer.isBuffer(content)) {
    dom = htmlparser.parseDOM(content, options);
  } else {
    dom = content;
  }

  return dom;
}
```
- example usage
```shell
...
*/
var htmlparser = require('htmlparser2');

/*
Parser
*/
exports = module.exports = function(content, options) {
var dom = exports.evaluate(content, options),
    // Generic root element
    root = exports.evaluate('<root></root>', options)[0];

root.type = 'root';

// Update the dom using the root
exports.update(dom, root);
...
```

#### <a name="apidoc.element.cheerio.parse.update"></a>[function <span class="apidocSignatureSpan">cheerio.parse.</span>update (arr, parent)](#apidoc.element.cheerio.parse.update)
- description and source-code
```javascript
update = function (arr, parent) {
  // normalize
  if (!Array.isArray(arr)) arr = [arr];

  // Update parent
  if (parent) {
    parent.children = arr;
  } else {
    parent = null;
  }

  // Update neighbors
  for (var i = 0; i < arr.length; i++) {
    var node = arr[i];

    // Cleanly remove existing nodes from their previous structures.
    var oldParent = node.parent || node.root,
        oldSiblings = oldParent && oldParent.children;
    if (oldSiblings && oldSiblings !== arr) {
      oldSiblings.splice(oldSiblings.indexOf(node), 1);
      if (node.prev) {
        node.prev.next = node.next;
      }
      if (node.next) {
        node.next.prev = node.prev;
      }
    }

    if (parent) {
      node.prev = arr[i - 1] || null;
      node.next = arr[i + 1] || null;
    } else {
      node.prev = node.next = null;
    }

    if (parent && parent.type === 'root') {
      node.root = parent;
      node.parent = null;
    } else {
      node.root = null;
      node.parent = parent;
    }
  }

  return parent;
}
```
- example usage
```shell
...
var dom = exports.evaluate(content, options),
    // Generic root element
    root = exports.evaluate('<root></root>', options)[0];

root.type = 'root';

// Update the dom using the root
exports.update(dom, root);

return root;
};

exports.evaluate = function(content, options) {
// options = options || $.fn.options;
...
```



# <a name="apidoc.module.cheerio.static"></a>[module cheerio.static](#apidoc.module.cheerio.static)

#### <a name="apidoc.element.cheerio.static.contains"></a>[function <span class="apidocSignatureSpan">cheerio.static.</span>contains (container, contained)](#apidoc.element.cheerio.static.contains)
- description and source-code
```javascript
contains = function (container, contained) {

  // According to the jQuery API, an element does not "contain" itself
  if (contained === container) {
    return false;
  }

  // Step up the descendants, stopping when the root element is reached
  // (signaled by '.parent' returning a reference to the same object)
  while (contained && contained !== contained.parent) {
    contained = contained.parent;
    if (contained === container) {
      return true;
    }
  }

  return false;
}
```
- example usage
```shell
...
Sometimes you need to work with the top-level root element. To query it, you can use '$.root()'.

'''js
$.root().append('<ul id="vegetables"></ul>').html();
//=> <ul id="fruits">...</ul><ul id="vegetables"></ul>
'''

#### $.contains( container, contained )
Checks to see if the 'contained' DOM element is a descendant of the 'container' DOM element.

#### $.parseHTML( data [, context ] [, keepScripts ] )
Parses a string into an array of DOM nodes. The 'context' argument has no meaning for Cheerio, but it is maintained for API compatability
.

#### $.load( html[, options ] )
Load in the HTML. (See the previous section titled "Loading" for more information.)
...
```

#### <a name="apidoc.element.cheerio.static.html"></a>[function <span class="apidocSignatureSpan">cheerio.static.</span>html (dom, options)](#apidoc.element.cheerio.static.html)
- description and source-code
```javascript
html = function (dom, options) {
  var Cheerio = require('./cheerio');

  // be flexible about parameters, sometimes we call html(),
  // with options as only parameter
  // check dom argument for dom element specific properties
  // assume there is no 'length' or 'type' properties in the options object
  if (Object.prototype.toString.call(dom) === '[object Object]' && !options && !('length' in dom) && !('type' in dom))
  {
    options = dom;
    dom = undefined;
  }

  // sometimes $.html() used without preloading html
  // so fallback non existing options to the default ones
  options = _.defaults(options || {}, this._options, Cheerio.prototype.options);

  return render(this, dom, options);
}
```
- example usage
```shell
...
'''js
let cheerio = require('cheerio')
let $ = cheerio.load('<h2 class="title">Hello world</h2>')

$('h2.title').text('Hello there!')
$('h2').addClass('welcome')

$.html()
//=> <h2 class="title welcome">Hello there!</h2>
'''

## Installation
'npm install cheerio'

## Features
...
```

#### <a name="apidoc.element.cheerio.static.load"></a>[function <span class="apidocSignatureSpan">cheerio.static.</span>load (content, options)](#apidoc.element.cheerio.static.load)
- description and source-code
```javascript
load = function (content, options) {
  var Cheerio = require('./cheerio');

  options = _.defaults(options || {}, Cheerio.prototype.options);

  var root = parse(content, options);

  var initialize = function(selector, context, r, opts) {
    if (!(this instanceof initialize)) {
      return new initialize(selector, context, r, opts);
    }
    opts = _.defaults(opts || {}, options);
    return Cheerio.call(this, selector, context, r || root, opts);
  };

  // Ensure that selections created by the "loaded" 'initialize' function are
  // true Cheerio instances.
  initialize.prototype = Object.create(Cheerio.prototype);
  initialize.prototype.constructor = initialize;

  // Mimic jQuery's prototype alias for plugin authors.
  initialize.fn = initialize.prototype;

  // Keep a reference to the top-level scope so we can chain methods that implicitly
  // resolve selectors; e.g. $("<span>").(".bar"), which otherwise loses ._root
  initialize.prototype._originalRoot = root;

  // Add in the static methods
  _.merge(initialize, exports);

  // Add in the root
  initialize._root = root;
  // store options
  initialize._options = options;

  return initialize;
}
```
- example usage
```shell
...
  </a>
</div>

<br />

'''js
let cheerio = require('cheerio')
let $ = cheerio.load('<h2 class="title">Hello world</h2>')

$('h2.title').text('Hello there!')
$('h2').addClass('welcome')

$.html()
//=> <h2 class="title welcome">Hello there!</h2>
'''
...
```

#### <a name="apidoc.element.cheerio.static.parseHTML"></a>[function <span class="apidocSignatureSpan">cheerio.static.</span>parseHTML (data, context, keepScripts)](#apidoc.element.cheerio.static.parseHTML)
- description and source-code
```javascript
parseHTML = function (data, context, keepScripts) {
  var parsed;

  if (!data || typeof data !== 'string') {
    return null;
  }

  if (typeof context === 'boolean') {
    keepScripts = context;
  }

  parsed = this.load(data);
  if (!keepScripts) {
    parsed('script').remove();
  }

  // The 'children' array is used by Cheerio internally to group elements that
  // share the same parents. When nodes created through 'parseHTML' are
  // inserted into previously-existing DOM structures, they will be removed
  // from the 'children' array. The results of 'parseHTML' should remain
  // constant across these operations, so a shallow copy should be returned.
  return parsed.root()[0].children.slice();
}
```
- example usage
```shell
...
$.root().append('<ul id="vegetables"></ul>').html();
//=> <ul id="fruits">...</ul><ul id="vegetables"></ul>
'''

#### $.contains( container, contained )
Checks to see if the 'contained' DOM element is a descendant of the 'container' DOM element.

#### $.parseHTML( data [, context ] [, keepScripts ] )
Parses a string into an array of DOM nodes. The 'context' argument has no meaning for Cheerio, but it is maintained for API compatability
.

#### $.load( html[, options ] )
Load in the HTML. (See the previous section titled "Loading" for more information.)

### Plugins
...
```

#### <a name="apidoc.element.cheerio.static.root"></a>[function <span class="apidocSignatureSpan">cheerio.static.</span>root ()](#apidoc.element.cheerio.static.root)
- description and source-code
```javascript
root = function () {
  return this(this._root);
}
```
- example usage
```shell
...
var moreFruit = $('#fruits').clone()
'''

### Utilities

#### $.root

Sometimes you need to work with the top-level root element. To query it, you can use '$.root()'.

'''js
$.root().append('<ul id="vegetables"></ul>').html();
//=> <ul id="fruits">...</ul><ul id="vegetables"></ul>
'''

#### $.contains( container, contained )
...
```

#### <a name="apidoc.element.cheerio.static.text"></a>[function <span class="apidocSignatureSpan">cheerio.static.</span>text (elems)](#apidoc.element.cheerio.static.text)
- description and source-code
```javascript
text = function (elems) {
  if (!elems) {
    elems = this.root();
  }

  var ret = '',
      len = elems.length,
      elem;

  for (var i = 0; i < len; i++) {
    elem = elems[i];
    if (elem.type === 'text') ret += elem.data;
    else if (elem.children && elem.type !== 'comment') {
      ret += exports.text(elem.children);
    }
  }

  return ret;
}
```
- example usage
```shell
...

<br />

'''js
let cheerio = require('cheerio')
let $ = cheerio.load('<h2 class="title">Hello world</h2>')

$('h2.title').text('Hello there!')
$('h2').addClass('welcome')

$.html()
//=> <h2 class="title welcome">Hello there!</h2>
'''

## Installation
...
```

#### <a name="apidoc.element.cheerio.static.xml"></a>[function <span class="apidocSignatureSpan">cheerio.static.</span>xml (dom)](#apidoc.element.cheerio.static.xml)
- description and source-code
```javascript
xml = function (dom) {
  var options = _.defaults({xmlMode: true}, this._options);

  return render(this, dom, options);
}
```
- example usage
```shell
...
'''xml
$ = cheerio.load('<media:thumbnail url="http://www.foo.com/keyframe.jpg" width="75" height="50" time="12:05:01.123"/>');
'''

... and later want to render to XML. To do this, you can use the 'xml' utility function:

'''js
$.xml()
//=>  <media:thumbnail url="http://www.foo.com/keyframe.jpg" width="75" height="50" time="12:05:01.123"/>
'''

You may also render the text content of a Cheerio object using the 'text' static method:

'''js
$ = cheerio.load('This is <em>content</em>.')
...
```



# <a name="apidoc.module.cheerio.utils"></a>[module cheerio.utils](#apidoc.module.cheerio.utils)

#### <a name="apidoc.element.cheerio.utils.camelCase"></a>[function <span class="apidocSignatureSpan">cheerio.utils.</span>camelCase (str)](#apidoc.element.cheerio.utils.camelCase)
- description and source-code
```javascript
camelCase = function (str) {
  return str.replace(/[_.-](\w|$)/g, function(_, x) {
    return x.toUpperCase();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cheerio.utils.cloneDom"></a>[function <span class="apidocSignatureSpan">cheerio.utils.</span>cloneDom (dom, options)](#apidoc.element.cheerio.utils.cloneDom)
- description and source-code
```javascript
cloneDom = function (dom, options) {
  return parse(render(dom, options), options).children;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cheerio.utils.cssCase"></a>[function <span class="apidocSignatureSpan">cheerio.utils.</span>cssCase (str)](#apidoc.element.cheerio.utils.cssCase)
- description and source-code
```javascript
cssCase = function (str) {
  return str.replace(/[A-Z]/g, '-$&').toLowerCase();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cheerio.utils.domEach"></a>[function <span class="apidocSignatureSpan">cheerio.utils.</span>domEach (cheerio, fn)](#apidoc.element.cheerio.utils.domEach)
- description and source-code
```javascript
domEach = function (cheerio, fn) {
  var i = 0, len = cheerio.length;
  while (i < len && fn.call(cheerio, i, cheerio[i]) !== false) ++i;
  return cheerio;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cheerio.utils.isHtml"></a>[function <span class="apidocSignatureSpan">cheerio.utils.</span>isHtml (str)](#apidoc.element.cheerio.utils.isHtml)
- description and source-code
```javascript
isHtml = function (str) {
  // Faster than running regex, if str starts with '<' and ends with '>', assume it's HTML
  if (str.charAt(0) === '<' && str.charAt(str.length - 1) === '>' && str.length >= 3) return true;

  // Run the regex
  var match = quickExpr.exec(str);
  return !!(match && match[1]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cheerio.utils.isTag"></a>[function <span class="apidocSignatureSpan">cheerio.utils.</span>isTag (type)](#apidoc.element.cheerio.utils.isTag)
- description and source-code
```javascript
isTag = function (type) {
  if (type.type) type = type.type;
  return tags[type] || false;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
