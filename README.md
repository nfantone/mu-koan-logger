# mu-kōän-logger 公案-ログ

[![Build Status](https://travis-ci.org/nfantone/mu-koan-logger.svg?branch=master)](https://travis-ci.org/nfantone/mu-koan-logger)

> A [winston][1] logger provider for [mu-kōän][2] applications.

[![js-semistandard-style](https://cdn.rawgit.com/flet/semistandard/master/badge.svg)](https://github.com/Flet/semistandard)

```sh
npm i --save mu-koan-logger
```

### Usage
Returns a `winston.Logger` given an `options.logger` property and a set
of prioritized rules.
   
- If `options.logger` is a string, returns `winston.loggers.get(options.logger)`.
- If `options.logger` is a `winston.Logger` instance, returns that same instance.
- If it is neither, return winston's default logger.


```javascript
const logger = require('mu-koan-logger');

/**
 * Returns `winston.loggers.get('my-logger')`.
 */
var log = logger.get({ logger: 'my-logger' })
```


---

## License
MIT

[1]: https://www.npmjs.com/winston
[2]: https://www.npmjs.com/mu-koan
