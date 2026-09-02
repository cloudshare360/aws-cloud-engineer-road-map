# JavaScript Fundamentals: Variables and Data Types

## Overview

JavaScript is the foundation of Node.js. Before building server-side applications, you need to master core JavaScript concepts.

## Topics Covered

- Let, const, and var
- Data types
- Type conversion
- Variables in practice

## Variables: let, const, var

### var (Legacy)
```javascript
var name = "Alice";
var age = 30;
```
- Function-scoped
- Can be re-declared
- Hoisted to top of function

### let (Modern)
```javascript
let name = "Alice";
let age = 30;
```
- Block-scoped
- Cannot be re-declared in same scope
- Not hoisted (temporal dead zone)

### const (Constants)
```javascript
const PI = 3.14159;
const person = { name: "Alice", age: 30 };

// Object properties can change
person.name = "Bob";
// But you can't reassign the variable
// person = {} // Error!
```
- Block-scoped
- Cannot be reassigned
- For objects: properties/arrays can still be mutated

## Data Types

### Primitive Types

| Type | Example | Description |
|------|---------|-------------|
| `string` | `"hello"`, `'world'` | Text |
| `number` | `42`, `3.14` | Numbers |
| `bigint` | `123456789012345678901234567890n` | Large integers |
| `boolean` | `true`, `false` | True/false |
| `undefined` | `let x;` | Variable without value |
| `null` | `let x = null;` | Intentional empty |
| `symbol` | `Symbol("id")` | Unique identifiers |

```javascript
// Strings
const greeting = "Hello, World!";
const message = `Template literal with ${greeting}`;
const multiLine = `
  Line 1
  Line 2
`;

// Numbers
const integer = 42;
const float = 3.14;
const negative = -10;

// Boolean
const isActive = true;
const hasPermission = false;

// Undefined
let notAssigned;
console.log(notAssigned); // undefined

// Null
const explicitNull = null;

// Symbol
const id = Symbol("id");
```

### Reference Types (Objects)

```javascript
// Object
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

// Array
const numbers = [1, 2, 3, 4, 5];
const mixedArray = ["hello", 42, true, { key: "value" }];

// Function
const greet = function(name) {
  return `Hello, ${name}!`;
};

// Date
const now = new Date();
const birthday = new Date("1990-01-01");

// RegExp
const pattern = /hello/gi;
```

## Type Conversion

### Implicit (Automatic)
```javascript
// JavaScript converts types automatically
console.log("5" + 3); // "53" (number becomes string)
console.log("10" * 2); // 20 (string becomes number)
console.log("5" - 3); // 2 (string becomes number)
```

### Explicit (Manual)
```javascript
// String
const str = String(123); // "123"
const str2 = (456).toString(); // "456"

// Number
const num = Number("123"); // 123
const float = parseFloat("3.14"); // 3.14
const int = parseInt("42px", 10); // 42

// Boolean
const bool = Boolean(1); // true
const bool2 = Boolean(0); // false
```

## typeof Operator

```javascript
typeof "hello";      // "string"
typeof 42;           // "number"
typeof true;         // "boolean"
typeof undefined;    // "undefined"
typeof null;         // "object" (historical bug)
typeof {};           // "object"
typeof [];           // "object"
typeof function() {}; // "function"
typeof Symbol();     // "symbol"
typeof 123n;         // "bigint"
```

## Hands-on Exercises

### Exercise 1: Declare Variables
Declare variables for:
- A product name (string)
- Price (number)
- In stock (boolean)
- Null value for discontinued items
- Undefined for optional features

```javascript
// Solution
const productName = "Laptop";
let price = 999.99;
const inStock = true;
const discontinued = null;
let warranty; // undefined
```

### Exercise 2: Type Conversion
Convert a string "123" to a number, then back to a string. Calculate the sum of "123" and 456.

```javascript
// Solution
const strNum = "123";
const num = Number(strNum); // 123
const backToString = num.toString(); // "123"
const sum = Number("123") + 456; // 579
```

### Exercise 3: Data Type Checker
Write a function that takes a value and returns its data type:

```javascript
function checkType(value) {
  if (value === null) return "null";
  if (Array.isArray(value)) return "array";
  return typeof value;
}

console.log(checkType(null));        // "null"
console.log(checkType([1, 2, 3]));   // "array"
console.log(checkType("hello"));     // "string"
console.log(checkType(42));          // "number"
```

## Knowledge Check

1. What's the difference between `let` and `var`?
2. Is `null` a primitive or reference type?
3. What is the Temporal Dead Zone?
4. Why does `typeof null` return `"object"`?
5. Can you change the properties of a `const` object?

## Next Steps

- [Functions and Scope](./02-functions-and-scope.md)
- [Arrays and Objects](./03-arrays-and-objects.md)
- [Project: Todo App](../projects/todo-app.md)
