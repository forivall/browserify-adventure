With browserify, you can use a `require()` function to load code. `require()`
takes a string module path as its only argument, just like in node. For example:

    var a = require('aaa')

Here The `aaa` module is loaded and the value exported from `aaa` is saved into
the `a` variable.

When the module path begins with a "./", it is interpreted as path relative to
the currently executing file.

Write a program that loads `'foo.js'` from the local directory. `'foo.js'` will
export a single function as its exported value. Call the function exported by
foo.js with process.argv[2] as an argument and print the result with
console.log().