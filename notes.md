# React Notes
<!-- Always Run These commands to run React project-->
Every time you want to start your React project

<!-- Just run: -->
cd myapp
npm run dev

<!-- Whts is React-JS -->
React-JS is a JS Library used to make UI(User-Interface) build by facebook in 2013

<!-- Diff Between Library And Framework -->

<!-- Library                                                            Framework -->

You control the flow.                                ||     Framework controls the flow.

You call the library functions when you need them.   ||     It calls your code when needed.

No strict rules or structure.                        ||     Has strict rules and fixed structure.

More flexible and easier.                            ||     Less flexible but more complete. 

<!-- Import And Export   -->

<!-- Why we need export? -->
Because if a component stays inside 1 file, you cannot use it anywhere else.
<!-- Why we need import? -->
To use the exported component inside another file.

<!-- Types of Export -->

<!-- 1. Default Export -->
export default Button;

<!-- Imported like: -->
import Button from './Button';  

// In this we can use any variable name Like this to Import Button
import Btn from './Button';       // Using this also we can import the button

<!-- 2. Named Export -->
export const a = 10;

<!-- Imported like: -->
import { a } from './Button';//But In this we can use the correct variable name as write in the file
<!--Using default export=>we can only export single component in a file,
but using named export=> we do multiple -->

<!-- we cannot only import/Export components we can also import/export variables/functions -->


<!-- Real DOM vs Virtual DOM  -->

<!-- Real DOM (Browser DOM)                                          Virtual DOM (React) -->

Directly updates the actual webpage.               ||     A lightweight copy of the Real DOM.

Slow when many updates happen.                     ||     Fast — updates happen in memory first.

Every change reloads the entire part of the UI.    ||     Only the changed part goes to the Real DOM.


<!-- What is JSX -->

JSX is JavaScript + HTML combined together.
It allows you to write HTML inside JavaScript,

<!-- JSX Full-Form -->
In React Documentation there is no written that JSX fullform is this or that,they only write JSX is a syntax extension for javascript
In other websites they write its fullform is javascript XML.
But in this there is a confusion.


<!-- What is a component  -->

A component = HTML + CSS + JS all together in one small piece
that represents a part of your webpage.
<!-- Example -->

function Button(){
    return <button>Click me</button>;
}
<!-- diff between component or function -->

<!-- 1. Normal Function (Pure JavaScript) -->

A normal function is used to calculate something, return a value, or perform logic.
<!-- Example: -->
function add(a, b) {   
  return a + b;
}

<!-- 2. Component Function (React Component) -->

A component is also a function — but instead of returning a number or string, it returns UI (JSX).

<!-- Example: -->
function Button() {
  return <button>Click Me</button>;
}


