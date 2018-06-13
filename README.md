# truffle-expect
Simple module for ensuring expected parameters exist

-----------------------

### :warning: This repo is deprecated :warning:
**Truffle has moved all modules to a monorepo at [trufflesuite/truffle](https://github.com/trufflesuite/truffle). See you over there!**

-----------------------

### install

```
$ npm install truffle-expect
```

### Usage

```javascript
var expect = require("truffle-expect");

// The object you're testing
var options = {
  example: "exists"
  another: 5
};

expect.options(options, ["example", "another"]); // does nothing
expect.options(options, ["example", "another", "some_other_key"]); // errors because options["some_other_key"] is undefined
```
