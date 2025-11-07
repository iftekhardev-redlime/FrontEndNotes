Iftekhar Hyder

**undefined:** value not set yet
**null:** value set as empty by programmer

```javascript
console.log("asdasddas");
let userMsg = 'kary'; 
var userMsg1 = 'Yabibi'; // old

// '===' deos nto convert & checks for value + same type
// '==' coverts to same type and compares

```

```javascript
// default values in functions
function greetUser(msg = 'gekki'){
  console.log(msg);
}

// arrow functions : anonymous functions that does not need a name
onClick = {() => doSmth()} // does not carry any name


export default () => {
  console.log('Hello');
}

// objects and classes

const userName = 'Max';
const user = {
   name: "Max",
   age: 34
};

console.log(user.name); // using dot notation

// storing functions in objects
const user = {
   age: 34,
   greet(){
     console.log(this.age); // access this objects var
     return "GREET!";
   }
}

console.log(user.greet());

class User{ // capital case char it should be 
  constructor(name, age){
    this.name = name;
    this.age = age;
  }
  greet(){
    console.log("Hello i am " + this.name + ", how are you?");
  }
}// like a blue print

const user1 = new User("Manuel", 45);

user1.greet();

// arrays and array methods
const hobbies = ['sports', 'music', 'dancing']
console.log(hobbies[0]); // sports

hobbies.push("") // to add items to the array

const index = hobbies.findIndex((item) => {
   return item === "Sports".toLowerCase();
});

const index = hobbies.findIndex((item) => item === "Sports".toLowerCase()); // one line

console.log(hobbies[index]) // 0

const newHobbies = hobbies.map((item) => item + '!')
cosnt newHObj = hobbies.map((item) => {text: item}) // always return arrays
console.log(newHobbies);

// destructuring arrays

const [firstName, latName] = ["Max", "Guzi"] // firstName M lastName G

// destructuring objects
const {firstName, age} = {firstName: "Max", age: 34}

const {name: userName, age} = { // aliasing
  name: "max",
  age: 34
}

console.log(userName); // max

// Spread operator
const newHobbies = ['Reading'];
const mergedHobbies = [...hobbies, ...newHobbies] // pull out values from this array and merge the arrays : comma seperated values as new array


const extendedUser = {
  isAdmin: true,
  ...user // pull out key value pairs from user object and add it here
}


// for loop: looping through arrays using of
for (const hobby of hobbies) {
  console.log(hobby);
}

// Manipulating the DOM in JS : Document object model

cosnt list = document.querySelector('ul')
list.remove() // removes the item form DOM


// Using functions as values
const handleTimeout2 = () => {
  console.log("timed out again!");
}

setTimeout(handleTimeout2, 2000); // passing as values
setTimeout(handleTimeout2()) // calls imediatelly : wrong thing to do


// function as parameter
function greeter(greeterFn){
  greetFn();
}

greeter(() => console.log("Hi"));


// premitives and reference values

// not stored in addres but stored in variables : callstack (faster access)
let userMessage = 'asdasd';
userMessage = 'HelloThere' + userMessage; // new string will be produced


// arrays are objects : reference values stored in heaps
const hobbies = ['Sports', 'Cooking'];
hobbies.push("Working"); // reach out to that address open the value in that address and add this new item to this new item in memory
console.log(hobbies);


Math.floor(1 + Math.random() * 3 + 1) // 1 - 3 it will return random

```

React Start:

```jsx
// Components: User interface building blocks
// creating component : functional
function Header(){
  return (
    <header>
     ....
    </header>
  );
}

function App(){
  return (<Header />);
}

export default App;


// importing and optimized import of images
import reactImg from './assets/image.png';

...
return <img src={reactImg} /> // always use image like this not using noraml path




```