# default [![Build Status](http://img.shields.io/travis/Safareli/default.svg)](http://travis-ci.org/Safareli/default) [![NPM version](https://badge-me.herokuapp.com/api/npm/default.png)](http://badges.enytc.com/for/npm/default) [![Code Climate](https://codeclimate.com/github/Safareli/default.png)](https://codeclimate.com/github/Safareli/default)

> extend object from default object or if it is undefined return default one

## Getting Started
Install the module with: `npm install default`

```javascript
require('default');

"tony".default("bob") // "bob"
"tony".default(null) // "tony"

({
    userName:'jhon555',
    gender:'male'
}).default({
    gender:'ather',
    type:'free'
});
//{
//    userName:'jhon555',
//    gender:'ather',
//    type:'free'
//}
```

## Documentation

#### Object.prototype.default(toCheck)

```javascript
myObj.default(toCheck);
```
The `default` method returns `myObj` if `toCheck` is `null` or `undefined`.
if `toCheck` and `myObj` are both objects it goes for each key in `myObj` and copies them into `toCheck` if it is not already defined .
in other cases it just returns `toCheck`.

see test file for more details


## License 

The MIT License

Copyright (c) 2014, Irakli Safareli

Permission is hereby granted, free of charge, to any person
obtaining a copy of this software and associated documentation
files (the "Software"), to deal in the Software without
restriction, including without limitation the rights to use,
copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following
conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.
