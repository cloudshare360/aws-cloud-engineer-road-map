# JavaScript Fundamentals: Functions and Scope

## Overview

Functions are the building blocks of JavaScript. Understanding scope is crucial for writing clean, bug-free code.

## Topics Covered

- Function declarations and expressions
- Arrow functions
- Scope and closure
- Higher-order functions
- Callback functions

## Function Declarations

```javascript
// Function declaration (hoisted)
function greet(name) {
  return `Hello, ${name}!`;
}

// Called before declared works
console.log(greet("Alice")); // "Hello, Alice!"

// Function expression
const greet = function(name) {
  return `Hello, ${name}!`;
};

// Arrow function (ES6)
const greet = (name) => {
  return `Hello, ${name}!`;
};

// Concise arrow function
const greet = (name) => `Hello, ${name}!`;

// No parameters
const greet = () => `Hello!`;

// Single parameter (parentheses optional)
const greet = name => `Hello, ${name}!`;
```

## Parameters and Arguments

```javascript
// Default parameters (ES6)
function greet(name = "Guest", greeting = "Hello") {
  return `${greeting}, ${name}!`;
}

console.log(greet()); // "Hello, Guest!"
console.log(greet("Bob")); // "Hello, Bob!"

// Rest parameters (ES6)
function sum(...numbers) {
  return numbers.reduce((acc, num) => acc + num, 0);
}

console.log(sum(1, 2, 3, 4, 5)); // 15

// Arguments object (non-arrow functions)
function showArgs() {
  console.log(arguments);
}
```

## Scope

### Global Scope
```javascript
const globalVar = "I'm global";

function myFunction() {
  console.log(globalVar); // Accessible
}
```

### Function Scope
```javascript
function myFunction() {
  const functionVar = "I'm function-scoped";
  
  if (true) {
    var blockVar = "I'm function-scoped (var)"; // var ignores block scope
    let blockLet = "I'm block-scoped (let)";
    const blockConst = "I'm block-scoped (const)";
  }
  
  console.log(blockVar); // "I'm function-scoped (var)"
  console.log(blockLet); // ReferenceError: blockLet is not defined
}
```

### Block Scope
```javascript
{
  let blockScoped = "Accessible within this block";
  const alsoBlockScoped = "Also accessible within this block";
  var functionScoped = "Not block-scoped (var)";
  
  console.log(blockScoped);     // Works
  console.log(alsoBlockScoped); // Works
}

console.log(functionScoped);    // Works (var)
console.log(blockScoped);       // ReferenceError
```

## Closure

A closure is a function that "remembers" its lexical scope.

```javascript
function createCounter() {
  let count = 0;
  
  return function() {
    count++;
    console.log(`Count: ${count}`);
  };
}

const counter = createCounter();
counter(); // "Count: 1"
counter(); // "Count: 2"
counter(); // "Count: 3"

// The inner function "closes over" the count variable
```

## Higher-Order Functions

Functions that take other functions as arguments or return functions.

```javascript
// Array methods (higher-order functions)
const numbers = [1, 2, 3, 4, 5];

// forEach
numbers.forEach(num => console.log(num));

// map
const doubled = numbers.map(num => num * 2); // [2, 4, 6, 8, 10]

// filter
const evens = numbers.filter(num => num % 2 === 0); // [2, 4]

// reduce
const sum = numbers.reduce((acc, curr) => acc + curr, 0); // 15

// find
const found = numbers.find(num => num > 3); // 4

// some/every
const hasLarge = numbers.some(num => num > 4); // true
const allSmall = numbers.every(num => num < 10); // true
```

## Callback Functions

```javascript
// Synchronous callback
function processData(data, callback) {
  const processed = data.map(item => item.toUpperCase());
  callback(processed);
}

processData(["hello", "world"], (result) => {
  console.log(result); // ["HELLO", "WORLD"]
});
```

## this Keyword

```javascript
// Regular function - this depends on how it's called
const person = {
  name: "Alice",
  greet: function() {
    return `Hello, I'm ${this.name}`;
  }
};

console.log(person.greet()); // "Hello, I'm Alice"

// Arrow function - this is inherited from lexical scope
const arrowGreet = () => {
  return `Hello, I'm ${this.name}`;
};

// this in arrow function is inherited from outer scope
// If defined at top level, this = global (or undefined in modules)
```

## IIFE (Immediately Invoked Function Expression)

```javascript
(function() {
  const privateVar = "I'm private";
  console.log(privateVar);
})();

// ES6 with arrow function
(() => {
  const privateVar = "I'm private";
  console.log(privateVar);
})();
```

## Hands-on Exercises

### Exercise 1: Function Types
Create three versions of a function that adds two numbers: regular function, function expression, and arrow function.

### Exercise 2: Scope Quiz
```javascript
let counter = 0;

function increment() {
  counter++;
}

function getPrivateCounter() {
  let privateCount = 0;
  return function() {
    privateCount++;
    return privateCount;
  };
}

const privateCounter = getPrivateCounter();
increment();
increment();
console.log(counter);
console.log(privateCounter());
console.log(privateCounter());
```

**What does this print?**
- counter: `2`
- privateCounter(): `1`
- privateCounter(): `2`

### Exercise 3: Closure-based Module
Create a `createBankAccount` function using closures that supports deposit, withdraw, and getBalance:

```javascript
const account = createBankAccount(100);
account.deposit(50);
account.withdraw(30);
console.log(account.getBalance()); // 120
```

## Knowledge Check

1. What's the difference between function declarations and expressions?
2. When would you use an arrow function vs a regular function?
3. What is the Temporal Dead Zone for `let`/`const`?
4. What is a closure and why is it useful?
5. What does `this` refer to in an arrow function?

## Next Steps

- [Arrays and Objects](./03-arrays-and-objects.md)
- [Async Await and Promises](./04-async-await-promises.md)
- [Functions and Scope - Project: Bank Account](./exercises/bank-account.md)
