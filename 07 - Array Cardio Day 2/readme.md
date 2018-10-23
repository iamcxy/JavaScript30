## Array Cardio Day

### Array.prototype.some()
The some() method tests wheather at least one element in the array passes the test impelmented by the provided function. 

some() executes the callback function once for each element present in the array until it finds one where callback returns a truthy value (a value that becomes true when converted to a Boolean). If such an element is found, some() immediately returns true. Otherwise, some() returns false. callback is invoked only for indexes of the array which have assigned values; 

### Array.prototype.every()
Return boolean value checking if every element in the array meet certain criteria


### Array.prototype.find()
Find is like filter, but instead returns just the one you are looking for

### Array.prototype.splice()
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice

find the index to remove then use `comments.splice(index,1)` to remove the element. 1 means remove one element at the index. 

### Array.prototype.slice()
```
    const newComments = [
      ...comments.slice(0, index),
      ...comments.slice(index+1)
    ];
```