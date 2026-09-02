# Node.js Introduction & Fundamentals

## Overview

Node.js is a JavaScript runtime built on Chrome's V8 JavaScript engine. It allows you to run JavaScript on the server side, making it possible to develop full-stack applications using a single programming language.

## What is Node.js?

- **Runtime**: Execution environment for JavaScript outside the browser
- **Built on**: V8 JavaScript engine (same as Chrome)
- **I/O Model**: Non-blocking, event-driven I/O
- **Event Loop**: Single-threaded event loop with async I/O

## Why Node.js?

| Advantage | Description |
|-----------|-------------|
| **Single Language** | Use JavaScript for both frontend and backend |
| **Non-blocking I/O** | Handle multiple requests concurrently |
| **NPM Ecosystem** | Largest package registry in the world |
| **Fast Startup** | V8 engine provides fast execution |
| **Community** | Large, active open-source community |
| **Microservices** | Excellent for building microservices |

## Event Loop

Understanding the event loop is crucial for writing efficient Node.js code.

### The Call Stack
```javascript
console.log("First");
console.log("Second");
// Call stack: execute synchronously, one at a time
```

### Callback Queue
```javascript
console.log("First");

setTimeout(() => {
  console.log("Third"); // Goes to callback queue
}, 0);

console.log("Second");
// Output: First, Second, Third
```

### Event Loop Phases
```
┌──────────────────────────┐
│   Timers (setTimeout)    │
└──────────┬───────────────┘
           │
┌──────────▼───────────────┐
│ Pending Callbacks        │
└──────────┬───────────────┘
           │
┌──────────▼───────────────┐
│ Idle, Prepare            │
└──────────┬───────────────┘
           │
┌──────────▼───────────────┐
│ Poll (I/O Events)        │
└──────────┬───────────────┘
           │
┌──────────▼───────────────┐
│ Check (setImmediate)     │
└──────────┬───────────────┘
           │
┌──────────▼───────────────┐
│ Close Callbacks          │
└──────────┬───────────────┘
           │
      ┌────┘
      │ Back to Timers
```

### Microtasks vs Macrotasks
```javascript
console.log("1"); // Macrotask

setTimeout(() => {
  console.log("2"); // Macrotask
}, 0);

Promise.resolve().then(() => {
  console.log("3"); // Microtask - runs before setTimeout
})

process.nextTick(() => {
  console.log("4"); // Microtask - runs before Promise
});

console.log("5"); // Macrotask

// Output: 1, 5, 4, 3, 2
```

## Modules

### Core Modules
```javascript
// Built-in Node.js modules
const fs = require("fs"); // File system
const path = require("path"); // Path utilities
const http = require("http"); // HTTP server
const url = require("url"); // URL parsing
const os = require("os"); // OS information
const crypto = require("crypto"); // Cryptography
```

### CommonJS Module System
```javascript
// math.js - Export
const add = (a, b) => a + b;
const multiply = (a, b) => a * b;

module.exports = { add, multiply };
// Or: module.exports.add = add;
// Or: module.exports.multiply = multiply;

// app.js - Import
const { add, multiply } = require("./math");
console.log(add(2, 3)); // 5
```

### ES Modules (ESM)
```javascript
// In package.json: { "type": "module" }

// math.js - Export
export const add = (a, b) => a + b;
export default { add, multiply };

// Or named exports
export { add, multiply };
export * from "./other.js";

// app.js - Import
import { add } from "./math.js";
import mathDefault from "./math.js";
```

## Process and Global Objects

```javascript
// process object
console.log(process.pid); // Process ID
console.log(process.argv); // Command line arguments
console.log(process.env.NODE_ENV); // Environment variables
console.log(process.cwd()); // Current working directory

// __dirname and __filename (CommonJS only)
console.log(__dirname); // Directory name
console.log(__filename); // File name

// Global objects
console.log(globalThis); // Available in all modules
console.log(setTimeout); // Global function
```

## Package Management

### package.json
```json
{
  "name": "my-node-app",
  "version": "1.0.0",
  "description": "My Node.js application",
  "main": "index.js",
  "scripts": {
    "start": "node index.js",
    "dev": "nodemon index.js",
    "test": "jest"
  },
  "dependencies": {
    "express": "^4.18.0"
  },
  "devDependencies": {
    "jest": "^29.0.0",
    "nodemon": "^2.0.0"
  }
}
```

### npm Commands
```bash
npm init          # Create package.json
npm install       # Install all dependencies
npm install <package> # Install a package
npm install -g <package> # Install globally
npm uninstall <package> # Remove a package
npm update        # Update packages
npm list          # List installed packages
npm audit         # Check for security vulnerabilities
npx <command>     # Run package command without installing globally
```

## Debugging

```bash
# Inspect mode
node --inspect=9229 app.js

# Chrome DevTools
chrome://inspect

# VS Code debugging
# Add .vscode/launch.json configuration
```

```json
// .vscode/launch.json
{
  "version": "0.2.0",
  "configurations": [
    {
      "type": "node",
      "request": "launch",
      "name": "Debug App",
      "program": "${workspaceFolder}/index.js"
    }
  ]
}
```

## Hands-on Exercises

### Exercise 1: Hello World Server
Create a simple HTTP server using Node.js built-in http module:

```javascript
const http = require("http");

const server = http.createServer((req, res) => {
  res.writeHead(200, { "Content-Type": "text/plain" });
  res.end("Hello World");
});

server.listen(3000, () => {
  console.log("Server running on port 3000");
});
```

### Exercise 2: Event Loop Visualization
Create a script that demonstrates the event loop order:

```javascript
console.log("1");
setTimeout(() => console.log("2"), 0);
Promise.resolve().then(() => console.log("3"));
process.nextTick(() => console.log("4"));
console.log("5");
```

### Exercise 3: Module Practice
Create two files:
1. `utils.js` - Export `formatDate`, `generateId`, and `calculateTotal`
2. `app.js` - Import and use these functions

## Knowledge Check

1. What is the difference between `require` and `import`?
2. What is the event loop and how does it work?
3. How do microtasks differ from macrotasks?
4. What is `__dirname` and how do you replicate it with ES modules?
5. How does `process.nextTick` differ from `Promise.then`?

## Next Steps

- [npm and Package Management](./08-npm-and-package-management.md)
- [File System Module](./09-file-system-module.md)
- [HTTP Server](./10-http-server.md)
- [Project: File Management API](./projects/file-api.md)

## Additional Resources

- [Node.js Deep Dive - YouTube Playlist](https://www.youtube.com/watch?v=pN6jk0uUrD8&list=PLxnjbfm5MCHFbRlyVCAqpJFdIzPN_IPID)
- [Programiz JavaScript Tutorials](https://www.programiz.com/javascript?utm_source=programiz.com&utm_medium=referral&utm_audience=ORGANIC-FREEMIUM&utm_campaign=course_promotion&utm_content=interests_learn_javascript&utm_term=nav_tutorials_banner)
