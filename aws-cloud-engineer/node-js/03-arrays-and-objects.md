# JavaScript Fundamentals: Arrays and Objects

## Overview

Arrays and objects are the two primary data structures in JavaScript. Mastering them is essential for any Node.js developer.

## Topics Covered

- Array methods
- Object methods
- Destructuring
- Spread and rest operators
- JSON serialization

## Arrays

### Array Basics
```javascript
const fruits = ["apple", "banana", "orange"];
const mixed = [1, "hello", true, { name: "Alice" }];

// Array length
console.log(fruits.length); // 3

// Access elements
console.log(fruits[0]); // "apple"
console.log(fruits[-1]); // undefined
console.log(fruits.at(-1)); // "orange" (ES2022)

// Modify arrays
fruits.push("grape"); // Add to end
fruits.unshift("kiwi"); // Add to beginning
fruits.pop(); // Remove from end
fruits.shift(); // Remove from beginning
```

### Array Methods

```javascript
const numbers = [1, 2, 3, 4, 5];

// map - transform each element
const doubled = numbers.map(n => n * 2); // [2, 4, 6, 8, 10]

// filter - select elements
const evens = numbers.filter(n => n % 2 === 0); // [2, 4]

// find - find first matching element
const found = numbers.find(n => n > 3); // 4

// findIndex - find index of first match
const index = numbers.findIndex(n => n > 3); // 3

// some - check if any element matches
const hasEven = numbers.some(n => n % 2 === 0); // true

// every - check if all elements match
const allPositive = numbers.every(n => n > 0); // true

// reduce - accumulate values
const sum = numbers.reduce((acc, curr) => acc + curr, 0); // 15

// forEach - iterate (no return value)
numbers.forEach(n => console.log(n));

// sort - sort elements
const sorted = [3, 1, 4, 1, 5].sort((a, b) => a - b); // [1, 1, 3, 4, 5]

// reverse - reverse array
const reversed = numbers.slice().reverse(); // [5, 4, 3, 2, 1]

// slice - extract portion
const part = numbers.slice(1, 3); // [2, 3]

// splice - modify in place
const modified = [1, 2, 3, 4, 5];
modified.splice(2, 1, "a", "b"); // [1, 2, "a", "b", 4, 5]

// includes - check if element exists
const hasThree = numbers.includes(3); // true

// indexOf - find first index
const idx = numbers.indexOf(3); // 2
```

## Objects

### Object Basics
```javascript
const person = {
  name: "Alice",
  age: 30,
  isEmployed: true,
  skills: ["JavaScript", "Node.js"],
  address: {
    city: "New York",
    country: "USA"
  }
};

// Access properties
console.log(person.name); // "Alice"
console.log(person["age"]); // 30
console.log(person.address.city); // "New York"

// Add/modify properties
person.email = "alice@example.com";
person.age = 31;
delete person.isEmployed;

// Shorthand property names (ES6)
const name = "Bob";
const age = 25;
const user = { name, age }; // { name: "Bob", age: 25 }

// Computed property names (ES6)
const propName = "dynamicKey";
const obj = { [propName]: "value" }; // { dynamicKey: "value" }
```

### Object Methods
```javascript
const person = {
  name: "Alice",
  age: 30,
  greet: function() {
    return `Hi, I'm ${this.name}`;
  },
  // Shorthand method
  greet2() {
    return `Hi, I'm ${this.name}`;
  }
};

// Object.keys
console.log(Object.keys(person)); // ["name", "age", "greet", "greet2"]

// Object.values
console.log(Object.values(person)); // ["Alice", 30, function, function]

// Object.entries
for (const [key, value] of Object.entries(person)) {
  console.log(`${key}: ${value}`);
}

// Object.assign (shallow copy)
const copy = Object.assign({}, person);

// Object spread (shallow copy) - ES2018
const copy2 = { ...person };
const merged = { ...person, extra: "data" };
```

## Destructuring

### Array Destructuring
```javascript
const [a, b, c] = [1, 2, 3];
console.log(a, b, c); // 1 2 3

// Skip elements
const [first, , third] = [1, 2, 3];
console.log(first, third); // 1 3

// Default values
const [x = 10, y = 20] = [5];
console.log(x, y); // 5 20

// Swap variables
let a = 1, b = 2;
[a, b] = [b, a];
console.log(a, b); // 2 1

// Rest in destructuring
const [first, ...rest] = [1, 2, 3, 4, 5];
console.log(first); // 1
console.log(rest); // [2, 3, 4, 5]
```

### Object Destructuring
```javascript
const person = { name: "Alice", age: 30, country: "USA" };

// Basic destructuring
const { name, age } = person;
console.log(name); // "Alice"

// Rename while destructuring
const { name: fullName, age: yearsOld } = person;
console.log(fullName, yearsOld); // "Alice" 30

// Default values
const { city = "Unknown" } = person;
console.log(city); // "Unknown"

// Nested destructuring
const user = {
  name: "Bob",
  address: { city: "NYC", zip: 10001 }
};
const { address: { city, zip } } = user;
console.log(city, zip); // "NYC" 10001
```

## Spread Operator (...)

```javascript
// Spread in arrays
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const combined = [...arr1, ...arr2]; // [1, 2, 3, 4, 5, 6]

// Spread in function calls
Math.max(...[1, 5, 3, 9, 2]); // 9

// Spread in objects (ES2018)
const defaults = { name: "Guest", age: 0 };
const person = { ...defaults, name: "Alice" };
// Result: { name: "Alice", age: 0 }
```

## JSON

```javascript
// JSON.stringify - object to string
const person = { name: "Alice", age: 30 };
const json = JSON.stringify(person); // '{"name":"Alice","age":30}'

// JSON.stringify with formatting
const pretty = JSON.stringify(person, null, 2);
// {
//   "name": "Alice",
//   "age": 30
// }

// JSON.parse - string to object
const parsed = JSON.parse(json); // { name: "Alice", age: 30 }

// Handle circular references
const circular = { name: "test" };
circular.self = circular;
// JSON.stringify(circular); // TypeError!

// Use replacer function for complex objects
const safeJson = JSON.stringify(obj, (key, value) => {
  if (key === "self") return undefined;
  return value;
});
```

## Hands-on Exercises

### Exercise 1: Array Operations
Create a function that takes an array of products (objects with price, name, category) and:
- Returns products over $100
- Groups products by category
- Calculates total price
- Sorts by price descending

### Exercise 2: Deep Cloning
Implement a function to deep clone an object without using JSON.parse/JSON.stringify:

```javascript
const deepClone = (obj) => {
  // Your code here
};

const original = { a: 1, b: { c: 2 } };
const copy = deepClone(original);
copy.b.c = 99;
console.log(original.b.c); // Should still be 2
```

## Knowledge Check

1. What's the difference between `slice()` and `splice()`?
2. How does object destructuring work with nested objects?
3. What is the spread operator a shorthand for?
4. Is `JSON.parse(JSON.stringify(obj))` always safe for cloning?
5. What's the difference between shallow and deep copy?

## Next Steps

- [Async Await and Promises](./04-async-await-promises.md)
- [ES6 Features in Depth](./05-es6-features.md)
