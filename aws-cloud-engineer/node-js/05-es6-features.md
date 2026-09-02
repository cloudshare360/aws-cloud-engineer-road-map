# JavaScript Fundamentals: ES6+ Features

## Overview

ES6 (ECMAScript 2015) revolutionized JavaScript. These features are essential for modern Node.js development.

## Topics Covered

- let/const vs var
- Template literals
- Destructuring
- Spread and rest operators
- Arrow functions
- Default parameters
- Modules (import/export)
- Classes
- Promises (covered separately)

## let/const vs var

Already covered in [01-variables-and-data-types.md](./01-variables-and-data-types.md)

## Template Literals

```javascript
// String interpolation
const name = "Alice";
const age = 30;
const message = `Hello, my name is ${name} and I'm ${age} years old.`;

// Multi-line strings
const html = `
  <div>
    <h1>Welcome, ${name}!</h1>
    <p>Age: ${age}</p>
  </div>
`;

// Expression interpolation
const a = 5, b = 10;
console.log(`${a} + ${b} = ${a + b}`); // "5 + 10 = 15"

// Tagged template literals
function highlight(strings, ...values) {
  return strings.reduce((acc, str, i) => {
    return acc + str + (values[i] ? `<strong>${values[i]}</strong>` : "");
  }, "");
}

const emphasized = highlight`Hello, my name is ${name} and I'm ${age}.`;
```

## Destructuring

Already covered in [03-arrays-and-objects.md](./03-arrays-and-objects.md). Key points:
- Arrays: `const [a, b, c] = [1, 2, 3];`
- Objects: `const { name, age } = { name: "Alice", age: 30 };`
- Nested: `const { a: { b: { c } } } = { a: { b: { c: 1 } } };`
- Default values: `const { name = "Guest" } = user;`

## Spread and Rest Operators

### Spread (`...`)
```javascript
// Spread in arrays
const arr1 = [1, 2, 3];
const arr2 = [...arr1, 4, 5]; // [1, 2, 3, 4, 5]

// Spread in objects
const obj1 = { a: 1, b: 2 };
const obj2 = { ...obj1, c: 3 }; // { a: 1, b: 2, c: 3 }

// Spread in function calls
const nums = [1, 2, 3];
Math.max(...nums); // 3
```

### Rest (`...`)
```javascript
// Rest in function parameters
function sum(...numbers) {
  return numbers.reduce((acc, num) => acc + num, 0);
}

// Rest in destructuring
const [first, ...rest] = [1, 2, 3, 4, 5];
// first = 1, rest = [2, 3, 4, 5]

const { a, b, ...others } = { a: 1, b: 2, c: 3, d: 4 };
// a = 1, b = 2, others = { c: 3, d: 4 }
```

## Arrow Functions

Already covered in [02-functions-and-scope.md](./02-functions-and-scope.md). Key differences:
- No `this` binding (uses lexical scope)
- No `arguments` object
- Cannot be used as constructors
- Can't be used as methods that need their own `this`

## Default Parameters

```javascript
// ES6 default parameters
function greet(name = "Guest", greeting = "Hello") {
  return `${greeting}, ${name}!`;
}

console.log(greet()); // "Hello, Guest!"
console.log(greet("Alice")); // "Hello, Alice"
console.log(greet("Bob", "Hi")); // "Hi, Bob"

// Default parameters with destructuring
function createUser({ name = "Anonymous", age = 0, email = "" } = {}) {
  return { name, age, email };
}
```

## Enhanced Object Literals

```javascript
const name = "Alice";
const age = 30;

// Shorthand property names
const person = { name, age };

// Shorthand method names
const person = {
  name,
  age,
  // Instead of: greet: function() { ... }
  greet() {
    return `Hi, I'm ${name}`;
  }
};

// Computed property names
const dynamicKey = "email";
const person = {
  name,
  [dynamicKey]: "alice@example.com"
};
```

## for...of and for...in Loops

```javascript
// for...of (arrays, strings, etc.)
const numbers = [1, 2, 3];
for (const num of numbers) {
  console.log(num); // 1, 2, 3
}

// for...in (object properties)
const person = { name: "Alice", age: 30 };
for (const key in person) {
  console.log(key, person[key]);
  // name Alice
  // age 30
}

// Using for...of with index
for (const [index, num] of numbers.entries()) {
  console.log(index, num);
  // 0 1
  // 1 2
  // 2 3
}
```

## Modules (import/export)

### CommonJS (Node.js default)
```javascript
// math.js
const add = (a, b) => a + b;
const multiply = (a, b) => a * b;

module.exports = { add, multiply };
// Or: module.exports.default = { add, multiply };

// app.js
const { add, multiply } = require("./math");
// Or: const math = require("./math"); then math.add()
```

### ES Modules (import/export)
```javascript
// math.mjs (or in .mjs files)
export const add = (a, b) => a + b;
export const multiply = (a, b) => a * b;

export default { add, multiply };

// Or separate exports
export { add, multiply };

// app.mjs
import { add, multiply } from "./math.mjs";
import mathDefault, { add as addFunc } from "./math.mjs";
```

### Enabling ES Modules in Node.js
```bash
# In package.json
{
  "type": "module"
}

# Or use .mjs extension
```

## Classes

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  // Instance method
  greet() {
    return `Hello, I'm ${this.name}`;
  }

  // Static method
  static compare(p1, p2) {
    return p1.age - p2.age;
  }

  // Getter
  get birthYear() {
    return new Date().getFullYear() - this.age;
  }

  // Setter
  set name(value) {
    this._name = value.trim();
  }
  get name() {
    return this._name;
  }
}

// Inheritance
class Developer extends Person {
  constructor(name, age, skills) {
    super(name, age); // Call parent constructor
    this.skills = skills;
  }

  greet() {
    return `${super.greet()} and I'm a developer`;
  }
}

const dev = new Developer("Alice", 30, ["JavaScript", "Node.js"]);
console.log(dev.greet()); // "Hello, I'm Alice and I'm a developer"
```

## Optional Chaining and Nullish Coalescing

```javascript
// Optional chaining (?.)
const user = {
  name: "Alice",
  address: {
    city: "New York"
  }
};

console.log(user?.address?.city); // "New York"
console.log(user?.address?.zip); // undefined
console.log(user?.nonExistent?.property); // undefined (no error!)

// Nullish coalescing (??)
const name = user.name || "Anonymous"; // Uses "Anonymous" if name is falsy
const name2 = user.name ?? "Anonymous"; // Uses "Anonymous" only if name is null/undefined

// Difference:
const count = 0;
const result1 = count || 10; // 10 (0 is falsy)
const result2 = count ?? 10; // 0 (0 is not null/undefined)
```

## Hands-on Exercises

### Exercise 1: Template Literals and Destructuring
Use the [Programiz JavaScript tutorials](https://www.programiz.com/javascript?utm_source=programiz.com&utm_medium=referral&utm_audience=ORGANIC-FREEMIUM&utm_campaign=course_promotion&utm_content=interests_learn_javascript&utm_term=nav_tutorials_banner) to practice template literals and destructuring.

### Exercise 2: Modules
Create two files:
1. `utils.js` - Export functions `formatName`, `calculateTax`
2. `app.js` - Import and use the functions

### Exercise 3: Classes
Create a `BankAccount` class with:
- Constructor accepting initial balance
- `deposit(amount)` method
- `withdraw(amount)` method with balance check
- `getBalance()` method
- Static method `createAccountNumber()`

## Knowledge Check

1. What does `?.` (optional chaining) do?
2. What's the difference between `||` and `??`?
3. How do ES modules differ from CommonJS modules?
4. Can you call a class constructor without `new`?
5. What is the spread operator a shorthand for?

## Next Steps

- [Async/Await and Promises](./04-async-await-promises.md)
- [Node.js Introduction](./07-nodejs-introduction.md)
