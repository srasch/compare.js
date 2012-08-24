# compare.js

compare.js implements JavaScript's comparison operators for Node.js and the browser the way you would expect them to be.

## Installation

    $ npm install compare.js

## Features

- Supports comparison of `number`, `string`, `boolean`, `function`, `object`, `array` and `undefined`.
- Supports comparison of native data types and constructor-created data types, such as `number` and `new Number()`.
- Supports comparison of objects and arrays using deep-equal.
- Supports comparison of objects and arrays with `<`, `<=`, `>` and `>=` by handling them as subsets.
- Supports comparison with `undefined` correctly, as `<=` and `>=` are problematic in plain JavaScript.
- Supports comparison in a perfectly type-safe way out-of-the-box.
- Supports comparison by equality and identity, depending on what makes sense.
- Developed using TDD and backed up by more than 690 unit tests.

## Quick Start

Basically, using compare.js is easy. All you need to do is to add a reference to it within your application:

### On Node.js

```javascript
var cmp = require('compare.js');
```

### In the browser

```html
<script type="text/javascript" src="https://raw.github.com/goloroden/compare.js/master/lib/index.js"></script>
```

### Common

Now you are able to use the various comparison operators. All you need to do is access the `cmp` object and
use its functions:

<table>
  <tr><th>Operator</th><th>Alias</th><th>Description</th></tr>
  <tr><td>cmp.eq(first, second)</td><td>cmp.equal(first, second)</td><td>equal</td></tr>
  <tr><td>cmp.ne(first, second)</td><td>cmp.notEqual(first, second)</td><td>not equal</td></tr>
  <tr><td>cmp.gt(first, second)</td><td>cmp.greaterThan(first, second)</td><td>greater than</td></tr>
  <tr><td>cmp.ge(first, second)</td><td>cmp.greaterThanOrEqual(first, second)</td><td>greater than or equal</td></tr>
  <tr><td>cmp.lt(first, second)</td><td>cmp.lessThan(first, second)</td><td>less than</td></tr>
  <tr><td>cmp.le(first, second)</td><td>cmp.lessThanOrEqual(first, second)</td><td>less than or equal</td></tr>
  <tr><td>cmp.id(first, second)</td><td>cmp.identical(first, second)</td><td>identical</td></tr>
</table>

Please note that each comparison operator works on each combination of types and does what you would expect it to do.

That's it :-)!

## Running the tests

Go to the folder where you have cloned compare.js to and run [mocha](https://github.com/visionmedia/mocha):

    $ mocha

## License

The MIT License (MIT)
Copyright (c) 2012 Golo Roden.
 
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.