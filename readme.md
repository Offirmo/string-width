# string-width [![Build Status](https://travis-ci.org/sindresorhus/string-width.svg?branch=master)](https://travis-ci.org/sindresorhus/string-width)

> Get the visual width of a string - the number of columns required to display it

Some Unicode characters are [fullwidth](https://en.wikipedia.org/wiki/Halfwidth_and_fullwidth_forms) and use double the normal width.

Useful to be able to measure the actual width of command-line output.


## Install

```
$ npm install --save string-width
```


## Usage

```js
var stringWidth = require('string-width');

stringWidth('古');
//=> 2

stringWidth('\u001b[1m古\u001b[22m');
//=> 2

stringWidth('a');
//=> 1
```


## Related

- [string-length](https://github.com/sindresorhus/string-length) - Get the real length of a string


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)
