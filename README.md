# class-nonew-decorator


[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
[![Build Status](https://travis-ci.org/direktspeed/class-nonew-decorator.svg?branch=master)](https://travis-ci.org/direktspeed/class-nonew-decorator)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
[![devDependency Status](https://david-dm.org/direktspeed/class-nonew-decorator/master/dev-status.svg)](https://david-dm.org/direktspeed/class-nonew-decorator/master#info=devDependencies)
[![Coverage Status](https://coveralls.io/repos/direktspeed/class-nonew-decorator/badge.svg?branch=master&service=github)](https://coveralls.io/github/direktspeed/class-nonew-decorator?branch=master)

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
