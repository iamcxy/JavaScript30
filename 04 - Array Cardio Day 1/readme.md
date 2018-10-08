## Working with JS arrays

practice using filter, map, sort, reduce, 

### Array.prototype.filter()
`filter()` iterate each element in the array and pass down the element to the callback function. Creates new array with all elements which passed the condition in the callback. 

### Array.prototype.map()
`map()` creates creates a new array with the results of calling provided callback function on iterating every single one of the element in the calling array. 

### Array.prototype.sort()
`sort()` uses `compareFunction(a , b)` to sort the element in the array. a comes first than b when compareFunction return -1, whereas b come first than a when compareFunction return 1, a & b stay unchanged with respect to each other when compareFunction return 0. 

|                            |     |
|----------------------------|-----|
| compareFunc(a,b) return -1 | a,b |
| compareFunc(a,b) return 1  | b,a |

### Array.prototype.reduce()
`reduce()` executes `reducer` function on each element of the array leading to single return value. the callback function receives four arguments `accumulator`, `currentValue`,`currentIndex`,`array`, keep in the mind that initialValue should be passed in most of the cases.

P.S If initialValue isn't provided, reduce() will execute the callback function starting at index 1, skipping the first index. If initialValue is provided, it will start at index 0.


### convert to Array object

`Arrayfrom(nodeList);` or `[...NodeList]` (es6)

### Misc
use `string.includes()` to check if the string contains another string
use `string.split` to split string to multiple elements 

`{}` is object and `[]` is array in JS

you can access object properties in two ways:
`objectName.propertyName`
`objectName["propertyName"]`