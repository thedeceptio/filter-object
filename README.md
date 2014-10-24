# filter-object [![NPM version](https://badge.fury.io/js/filter-object.svg)](http://badge.fury.io/js/filter-object)

> Return an object filtered to have only the keys that match the given glob patterns.

## Install
#### Install with [npm](npmjs.org):

```bash
npm i filter-object --save-dev
```

## Run tests

```bash
npm test
```

## Usage

```js
var filter = require('filter-object');

filter({a: 'a', b: 'b', c: 'c'}, '*')
//=> {a: 'a', b: 'b', c: 'c'}

filter({a: 'a', b: 'b', c: 'c'}, 'b')
//=> {b: 'b'}

filter({foo: 'a', bar: 'b', baz: 'c'}, 'b*')
//=> {bar: 'b', baz: 'c'}

filter({a: 'a', b: 'b', c: 'c'}, '{b,c}')
//=> {b: 'b', c: 'c'}
```

## Contributing
Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue][issues].

## Author

**Jon Schlinkert**
 
+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert) 

## License
Copyright (c) 2014 Jon Schlinkert, contributors.  
Released under the MIT license

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on October 24, 2014._

[issues]: https://github.com/jonschlinkert/filter-keys/issues