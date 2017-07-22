# class-nonew-decorator
[![Build Status][build]][link]]
[![semantic-release][semantic-image] ][semantic-url]
[build]: https://travis-ci.org/direktspeed/class-nonew-decorator.svg?branch=master
[link]: https://travis-ci.org/direktspeed/class-nonew-decorator
[semantic-image]: https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg
[semantic-url]: https://github.com/semantic-release/semantic-release

Allows to create an Instance from a JavaScript Class without invoking `new` keyword.

# Install

```bash
npm i class-nonew-decorator --save
```
# Use with ES6

```javascript
import nonew from 'class-nonew-decorator';

@nonew()
class IamClass {
    constructor() {
        console.log('IamClass Instance!');
    }
}

console.log(new IamClass() instanceof IamClass);  // true

console.log(IamClass() instanceof IamClass);  // true
```

# Use with CJS

```javascript
const nonew = require('class-nonew-decorator');

@nonew()
class IamClass {
    constructor() {
        console.log('IamClass Instance!');
    }
}

console.log(new IamClass() instanceof IamClass);  // true

console.log(IamClass() instanceof IamClass);  // true
```
