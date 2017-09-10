#react DOM
JSX class : `classname=" " `
JSX must `<br />`
JSX example : 
```
import React from 'react';
import ReactDOM from 'react-dom';

const theString = 'summary 2+3 = ';
ReactDOM.render(
    <h1>{theString+(2+3)}</h1>,
    document.getElementById('app')
);
```
JSX function / if else expression :
```
function coinToss() {
  // This function will randomly return either 'heads' or 'tails'.
  return Math.random() < 0.5 ? 'heads' : 'tails';
}

const pics = {
  kitty: 'https://s3.amazonaws.com/codecademy-content/courses/React/react_photo-kitty.jpg',
  doggy: 'https://s3.amazonaws.com/codecademy-content/courses/React/react_photo-puppy.jpeg'
};
const img;

// if/else expression :
const img = <img src={pics[coinToss() === 'heads' ? 'kitty' : 'doggy']} />;
ReactDOM.render(img, document.getElementById('app'))
```
JSX conditional expression :
```
const tasty = (
  <ul>
    <li>Applesauce</li>
    { !baby && <li>Pizza</li> }
    { age > 15 && <li>Brussels Sprouts</li> }
    { age > 20 && <li>Oysters</li> }
    { age > 25 && <li>Grappa</li> }
  </ul>
);
```
JSX .map
```
const strings = ['Home', 'Shop', 'About Me'];
const listItems = strings.map(string => <li>{string}</li>);

<ul>{listItems}</ul>
```
.map alternative
```
const liArray = [
  <li>item 1</li>, 
  <li>item 2<li>, 
  <li>item 3</li>
];

<ul>{liArray}</ul>
```
