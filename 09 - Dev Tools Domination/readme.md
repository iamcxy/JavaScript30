## Dev Tools Domination

### Attribute modification
use `attribute modification` to set a break point to see the function that modified the attribute of a tag.
See the function on `Souces` tab.

### Console.log

```
const dogs = [{ name: 'Snickers', age: 2 }, { name: 'hugo', age: 8 }];
```

//Interpolated
`console.log('Hello Iam a %s string!', 'test')`

//Styled
`console.log('I am some great text', 'font-size:50px;background:red')`

//Warning!
console.warn('OH NOOO');

//Error
console.error('Shit!');

//Info
console.info('Crocodiles eat 3-4 people per year');

//Testing
const p = document.querySelector('p');

console.assert( 1 === 1, 'That is wrong');
const p = document.querySelector('p');
console.assert(p.classList.contains('ouch'), 'That is wrong!');

// clearing
console.clear();

//View DOM elements
console.log(p);
console.dir(p);

// Grouping together
console.group(`${dog.name}`); or console.groupCollapsed(`${dog.name}`)
....
      console.log(`This is ${dog.name}`);
      console.log(`${dog.name} is ${dog.age} years old`);
      console.log(`${dog.name} is ${dog.age * 7} dog years old`);
console.groupEnd(`${dog.name}`);

// counting

console.count('Wes');
console.count('Wes');
console.count('Steve');


// timing
console.time('fetching data')
fetch('https://api.github.com/users/wesbos')
    .then(data => data.json())
    .then(data=>{
        console.timeEnd('fetching data');
        console.log(data);
    })

console.time();
console.timeEnd();

// table logging 
console.table(dogs);