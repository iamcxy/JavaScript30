## Type Ahead

### Fetch
we will use promise to get the response in es6 format `fetch(promise).then().then()....`
### Use spread to push to array
if an array is pushed to another array in this format: `a.push(b)`, a will contain b as nested arrays.
use es6 `spread` changes the array to each individual arguments, which in turn could push the elements of the array to another one. 

### Listen to input box event to display prompts 
Input change event only fire off when mouse clicked outside of the box, so `keyup` event should also be listened. 

calling `.join('')` on an array will turn the array into joint strings.(suited for HTML)


### Add commas to number
use ```function numberWithCommas(x) {
  return x.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ',');
}```  to add commas to the numbers