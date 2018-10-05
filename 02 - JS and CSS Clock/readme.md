## Clock in CSS and JS

Use Chrome console to experiment with different css properties under debugging tool->Sytles.

3 `<div>` with class `hand` are created to repsent sec, min, hour hands. 

`transition: all 0.5s;`
The transition property is specified as one or more single-property transitions, separated by commas. Each single-property transition describes the transition that should be applied to a single property (or the special values all and none). 

`transform-origin: 100%;` 
Set transform-origin at 100% to allow the hands to rotate at the origin of the clock. 

`transform`
We rotate the hand at 90 degree so the hands start 0 in the clock. 

transition make the elements change gradually and smoothly from one state to another, while transform move and change the appearce of the element. 

use `setInterval(func, delay)` to update the clock every second, and `Date()` object to get current time. Note that the function ref needs to be passed not the function execution`func()` with return. 

`transition-timing-function` entered under element.style of particular element in debugger tool would show a little icon to allow us tweak the function parameters to produce fun results.

`const hour_degree = (hour + (min/60) + (seconds/360))/12 * 360 + 90;` Degree calculation of hour should include the percentage lapsed in minutes and seconds within the hour. 

at 0 seconds the secondhand will transform from 354 degree back to 0 degree based on the math equation `((seconds / 60) * 360) + 90`. We simply tally the amount of degrees and keep on counting, so when it revisit 0 second it does show redundent backward transition ` seconds/60 * 360 + (hour * 360) + (min * 360) + 90`. Alternate solution is to change the time in transition to 0s temporarily. `transition: all 0.5s;`





