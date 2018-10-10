## JS Drum Kit

DEMO [HERE](https://cdn.rawgit.com/iamcxy/JavaScript30/c812f70e/01%20-%20JavaScript%20Drum%20Kit/index-PRACTICE.html) 

Each key is associated with a keycode. you can find the code conveniently at http://keycode.info. 

`data-key` attribute in HTML tags is used for JS to associate specified keystroke with specific audio and visual animations. 

`audio.currentTime = 0` rewind the sound to the start if the key is hit in succession over and over again.

DOM API `classList.add` is used to add `playing` attribute to activate scale animation

We also need to remove `playing` attribute after the transition has ended. Doable through setTimeout but we need to constantly sync(hardcode) the transition time in style sheet and in setTimeout, it's not very nice design. Better way to do this is listen to transition event end and then remove the `playing` tag. 

When you have an array/list of elements, you can't listen on all of them. We must explicitly loop over every singly element and attach an event listener. 

Use `console.log` to debug and learn anything. 

We will use `transitionend` event to remove playing after transition, `removeTransition` is created to remove the class. Multiple transition end event will happen, we only catch transform event which has the longest time. 

`this` is always on the element scope that called against the function, in this case `this` equals to the key that added event listener. 


