# [ix-cat](http://pubs.opengroup.org/onlinepubs/9699919799/utilities/cat.html) :cat2:

A POSIX-like `cat` in JavaScript.

[![NPM](https://nodei.co/npm/ix-cat.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/ix-cat/)

[![build status](https://secure.travis-ci.org/shama/ix-cat.svg)](https://travis-ci.org/shama/ix-cat)
[![Build status](https://ci.appveyor.com/api/projects/status/c15rf5fkw1g1cfqd)](https://ci.appveyor.com/project/shama/ix-cat)
[![NPM version](https://badge.fury.io/js/ix-cat.svg)](https://badge.fury.io/js/ix-cat)

<!-- [![browser support][https://ci.testling.com/shama/ix-cat.png]][https://ci.testling.com/shama/ix-cat] -->
[![Sauce Test Status](https://saucelabs.com/browser-matrix/shama.svg)](https://saucelabs.com/u/shama)

## CLI

```shell
echo "// before" | cat one.js two.js three.js > output.js
```

## API

```js
var Cat = require('ix-cat')
```

### `var cat = new Cat(argv)`
Returns a transform stream. `argv` can be:

* `_`: An array of arguments of file paths to concat; such as `cat one.js two.js three.js`
* `fs`: Override the file system with a node/io compatible fs.
* `u`: Write bytes without buffering.

# license
(c) 2015 Kyle Robinson Young. MIT License
