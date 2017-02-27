# hof-util-testdata
Generator for test fixtures

## Usage

The library contains a number of generators for values of certain types. Values are generators on accessing the type property.

### Example:

```js
const TestData = require('hof-util-testdata');

console.log(TestData.name);
// "David Fletcher"

console.log(TestData.name);
// "Irene O'Grady"
```

## Available generators

* `firstname`
* `lastname`
* `name`
* `email`
* `phone`
* `streetname`
* `streetsuffix`
* `address` - `${number(1,100)} ${streetname} ${streetsuffix}`
* `postcode`
* `country` - a random country from [homeoffice-countries](npmjs.com/homeoffice-countries)

## Functions

* `number(min, max)` - returns an integer between `min` and `max`
* `number(max)` - returns an integer between 0 and `max`
* `number()` - returns an integer between 0 and 100
