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










```