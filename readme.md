# obj-to-table [![Build Status](https://travis-ci.org/kevva/obj-to-table.svg?branch=master)](https://travis-ci.org/kevva/obj-to-table)

> Create a table from an array of objects


## Install

```
$ npm install --save obj-to-table
```


## Usage

```js
var objToTable = require('obj-to-table');

objToTable([{
	foo: 'bar',
	cat: 'meow',
	unicorn: 'moo'
}, {
	foo: 'crow',
	cat: 'eek',
	unicorn: 'buzz'
}, {
	foo: 'ow',
	cat: 'hee-haw',
	unicorn: 'hum'
}]);

console.log(table.toString());

/*
┌──────────────┬──────────────┬──────────────┐
│ foo          │ cat          │ unicorn      │
├──────────────┼──────────────┼──────────────┤
│ bar          │ meow         │ moo          │
├──────────────┼──────────────┼──────────────┤
│ crow         │ eek          │ buzz         │
├──────────────┼──────────────┼──────────────┤
│ ow           │ hee-haw      │ hum          │
└──────────────┴──────────────┴──────────────┘
*/
```


## API

### objToTable(data, [options])

#### data

*Required*  
Type: `array`, `object`

An array of objects containing your data.

#### options

Type: `object`

See the [cli-table](https://github.com/Automattic/cli-table) options.


## License

MIT © [Kevin Martensson](http://github.com/kevva)
