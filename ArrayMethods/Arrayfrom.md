# Array Methods  =>
-----------------------
&nbsp;

## Array.from()
------------------------------------------------------------
The Array.from() method creates a new, shallow-copied Array instance from an array-like or iterable object.
&nbsp;
 ### javascript demo
 ----------------------

```
console.log(Array.from('Hardik'));
// expected output: Array ["H", "a", "r","d","i","k"]

console.log(Array.from([1, 2, 3], x => x + x));
// expected output: Array [2, 4, 6]
```
### Syntax
-------------
```
Array.from(arrayLike[, mapFn[, thisArg]])
```
&nbsp;

### Parameters
-------------------------------------------------------

* **arraylike** 
An arraylike or iterable object to convert into an array
* **mapfn**(*optional*)
map function to call on every element in an array
* **thisArg**(*optional*)
value to use this when using map function

&nbsp;
### Description
*********************************************
Array.from() lets you create Arrays from: 

* array-like objects (objects with a length property and indexed elements) or
* iterable objects (objects where you can get its elements, such as Map and Set).

&nbsp;
### Examples
----------------------------

```
Array.from('foo'); 
// [ "f", "o", "o" ]
```


using map:
```
const map = new Map([[1, 2], [2, 4], [4, 8]]);
Array.from(map);
// [[1, 2], [2, 4], [4, 8]]

const mapper = new Map([['1', 'a'], ['2', 'b']]);
Array.from(mapper.values());
// ['a', 'b'];

Array.from(mapper.keys());
// ['1', '2
```
from arraylike-objects(function-arguments)
```
function f() {
  return Array.from(arguments);
}

f(1, 2, 3);

// [ 1, 2, 3 ]
```
using arrow functions (lambda of javascript)
```
Array.from([1,2,3],x=>x+x);
// [2, 4, 6]

// Generate a sequence of numbers
// Since the array is initialized with `undefined` on each position,
// the value of `v` below will be `undefined`
Array.from({length: 5}, (v, i) => i);
// [0, 1, 2, 3, 4]

```

Thanks for reading
