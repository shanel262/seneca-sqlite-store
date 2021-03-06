![Seneca](http://senecajs.org/files/assets/seneca-logo.png)
> A [Seneca.js](https://github.com/senecajs/) a seneca-auth plugin

# seneca-sqlite-store
[![npm version][npm-badge]][npm-url]
[![Build Status][travis-badge]][travis-url]
[![Dependency Status][david-badge]][david-url]
[![Coveralls][BadgeCoveralls]][Coveralls]
[![Gitter chat][gitter-badge]][gitter-url]

## Description

Seneca-SQLite is a SQLite database driver for [Seneca](https://github.com/senecajs/) MVP toolkit
This project was sponsored by [nearForm](http://nearform.com).

### Seneca compatibility
Supports Seneca versions **1.x** and **2.x**

## Install

```sh
npm install seneca-sqlite-store
```

## Using sqlite-store

When using seneca-auth the local auth must be initialized using:

```
var seneca              = require('seneca');
    var senecaSQLiteStore   = require('seneca-sqlite');

    var senecaConfig = {}
    var senecaSQLiteStoreOpts = {
        database:'/path/to/seneca_sqlite.db'
    };

```
```
var si = seneca(senecaConfig);
   si.use(senecaSQLiteStore, senecaSQLiteStoreOpts);
   si.ready( function(){
       var product = si.make('product');
       ...
   });

```

## Contributing
The [Senecajs org][] encourage open participation. If you feel you can help in any way, be it with
documentation, examples, extra testing, or new features please get in touch.

## Test
To run tests, simply use npm:

```sh
npm run test
```

## License
Copyright (c) 2016, Marius Ursache and other contributors.
Licensed under [MIT][].


[npm-badge]: https://badge.fury.io/js/seneca-sqlite-store.svg
[npm-url]: https://badge.fury.io/js/seneca-sqlite-store
[david-badge]: https://david-dm.org/senecajs/seneca-sqlite-store.svg
[david-url]: https://david-dm.org/senecajs/seneca-sqlite-store
[gitter-badge]: https://badges.gitter.im/senecajs/seneca.png
[gitter-url]: https://gitter.im/senecajs/seneca
[travis-badge]: https://travis-ci.org/senecajs/seneca-sqlite-store.svg
[travis-url]: https://travis-ci.org/senecajs/seneca-sqlite-store
[MIT]: ./LICENSE.txt
[Senecajs org]: https://github.com/senecajs/
[Coveralls]: https://coveralls.io/github/senecajs/seneca-sqlite-store?branch=master
[BadgeCoveralls]: https://coveralls.io/repos/github/senecajs/seneca-sqlite-store/badge.svg?branch=master
