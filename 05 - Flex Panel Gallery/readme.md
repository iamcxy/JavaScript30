## Flex Panel Gallery

### nested flex panel

`display:flex` to start using flexbox.
`flex : 1;` will evenly distribute the flex boxes.
use `border: 1px solid red;` to debug the layout of the panels.
we will be nesting flex boxes in different levels. 


`flex-basis` - specifies the initial size of the flex item, before any available space is distributed according to the flex factors. Default value is the length zero
`flex-shrink` - specifies the "flex shrink factor" which determines how much the flex item will shrink relative to the rest of the flex items in the flex container when there isn't enough space on the row. 
`flex-grow` - specifies the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion. It dictates what amount of the available space inside the flex container the item should take up. 

### transform: translateY()
use `transform: translateY(0)` and `transform: translateY(-+100)` for text vertical transition. 

### this.classList.toggle
`this.classList.toggle('open')` toggles the class on/off of `this` tag. 


### transition end event type
After `transitionend` event we will toggle `open-active` for text translation. Use if statement to only translate after `flex-grow` has ended. 