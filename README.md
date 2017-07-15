# sexcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install sexcore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var sexcoreTasks = require('sexcore-build');

litecoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var sexcoreTasks = require('sexcore-build');
sexcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/sxcmarket/sexcore) on the main sexcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/sxcmarket/sexcore/blob/master/LICENSE).

Copyright 2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2016 The Litecoin Core Developers
Copyright 2017 The Sexcoin Core Developers
