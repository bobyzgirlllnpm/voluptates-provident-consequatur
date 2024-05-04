# Array Helpers for JavaScript

![npm](https://img.shields.io/npm/v/@bobyzgirlllnpm/voluptates-provident-consequatur?logo=npm)
![npm](https://img.shields.io/npm/dm/@bobyzgirlllnpm/voluptates-provident-consequatur?logo=npm)

## What is this?

A collection of functions for working with arrays inspired by the methods that are available in Swift

## Usage

### Import

You need to import the methods first. Example:

```js
// ES6 module
import '@bobyzgirlllnpm/voluptates-provident-consequatur'

// node.js
require('@bobyzgirlllnpm/voluptates-provident-consequatur')
```

### firstIndex

Finds the index of the first element matching the predicate.
Example:

```js
const array = [5, 3, 7, 12]
const index = firstIndex(array, x => x <= 4) // 1
```

### firstWhere

Finds the first element matching the predicate (similar to `firstIndex`).
Example:

```js
const array = [5, 3, 7, 12]
const firstElementMatchingPredicate = firstWhere(array, x => x <= 4) // 3
```

### compactMap

Maps all values, filtering `null` or `undefined` values out
Example:

```js
const array = [
  { name: 'Henrik' },
  { name: 'Henrik', lastName: 'Panhans' },
  { name: 'Henrik' },
  { name: 'Henrik' }
]
const lastNames = compactMap(array, value => value.lastName) // ["Panhans"]
```
