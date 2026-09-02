# JavaScript Fundamentals: Async/Await and Promises

## Overview

Asynchronous programming is essential for Node.js. Understanding Promises and async/await is the key to writing efficient, non-blocking code.

## Topics Covered

- Callbacks vs Promises
- Promise chaining
- async/await syntax
- Error handling
- Promise methods

## The Problem with Callbacks

```javascript
// Callback hell / Pyramid of Doom
getUser(1, (err, user) => {
  if (err) throw err;
  getPosts(user.id, (err, posts) => {
    if (err) throw err;
    getComments(posts[0].id, (err, comments) => {
      if (err) throw err;
      console.log(comments);
    });
  });
});
```

## Promises

A Promise is an object representing the eventual completion or failure of an asynchronous operation.

```javascript
// Creating a promise
const promise = new Promise((resolve, reject) => {
  // Simulate async operation
  setTimeout(() => {
    const success = true;
    if (success) {
      resolve("Operation completed!");
    } else {
      reject(new Error("Operation failed!"));
    }
  }, 1000);
});

// Consuming a promise
promise
  .then(result => {
    console.log(result); // "Operation completed!"
  })
  .catch(error => {
    console.error(error.message); // "Operation failed!"
  })
  .finally(() => {
    console.log("Cleanup");
  });
```

### Promise States

1. **pending**: Initial state, neither fulfilled nor rejected
2. **fulfilled**: Operation completed successfully
3. **rejected**: Operation failed

```javascript
const promise = new Promise((resolve, reject) => {
  // Promise is pending here
  
  setTimeout(() => {
    resolve("Done!"); // Now fulfilled
    // Or: reject(new Error("Failed!")); // Now rejected
  }, 1000);
});
```

### Promise Chaining

```javascript
fetchUser(1)
  .then(user => {
    console.log("User:", user);
    return fetchPosts(user.id);
  })
  .then(posts => {
    console.log("Posts:", posts);
    return fetchComments(posts[0].id);
  })
  .then(comments => {
    console.log("Comments:", comments);
  })
  .catch(error => {
    console.error("Error:", error);
  });
```

### Promise Methods

```javascript
// Promise.all - wait for ALL promises to resolve
const p1 = Promise.resolve(3);
const p2 = 42;
const p3 = new Promise((resolve) => setTimeout(() => resolve("slow"), 100));

Promise.all([p1, p2, p3])
  .then(values => console.log(values)); // [3, 42, "slow"]

// Promise.race - first promise to settle
Promise.race([p1, p3])
  .then(value => console.log(value)); // 3 (p1 resolves first)

// Promise.allSettled - all promises, regardless of outcome
Promise.allSettled([Promise.resolve(1), Promise.reject("error")])
  .then(results => console.log(results));
  // [{status: "fulfilled", value: 1}, {status: "rejected", reason: "error"}]

// Promise.any - first promise to fulfill
Promise.any([Promise.reject("err"), Promise.resolve("success")])
  .then(value => console.log(value)); // "success"
```

## async/await

Syntactic sugar over Promises that makes asynchronous code look synchronous.

```javascript
// Async function always returns a Promise
async function fetchUser(id) {
  return { id, name: "Alice" };
}

// Equivalent to:
// function fetchUser(id) {
//   return Promise.resolve({ id, name: "Alice" });
// }

// Await waits for a Promise to resolve
async function getPosts(userId) {
  const response = await fetch(`/api/users/${userId}/posts`);
  const posts = await response.json();
  return posts;
}
```

### Async/Await vs Promise Chaining

```javascript
// With Promises
function getUserData(userId) {
  return fetchUser(userId)
    .then(user => fetchPosts(user.id))
    .then(posts => fetchComments(posts[0].id))
    .then(comments => ({ user, posts, comments }))
    .catch(error => {
      console.error("Error:", error);
    });
}

// With async/await
async function getUserData(userId) {
  try {
    const user = await fetchUser(userId);
    const posts = await fetchPosts(user.id);
    const comments = await fetchComments(posts[0].id);
    return { user, posts, comments };
  } catch (error) {
    console.error("Error:", error);
  }
}
```

## Error Handling

```javascript
async function riskyOperation() {
  try {
    const result = await mightFail();
    console.log("Success:", result);
  } catch (error) {
    if (error instanceof TypeError) {
      console.error("Type error:", error.message);
    } else {
      console.error("General error:", error);
    }
  } finally {
    console.log("Cleanup always runs");
  }
}

// Promise.all with error handling
async function fetchAll(urls) {
  const promises = urls.map(url => fetch(url));
  
  try {
    const results = await Promise.all(promises);
    return results;
  } catch (error) {
    console.error("One or more requests failed:", error);
    return null;
  }
}

// Handle partial failures with allSettled
async function fetchAllSafe(urls) {
  const promises = urls.map(url => 
    fetch(url).catch(err => ({ error: err, url }))
  );
  
  const results = await Promise.allSettled(promises);
  
  results.forEach((result, index) => {
    if (result.status === "fulfilled") {
      console.log(`URL ${index} succeeded`);
    } else {
      console.log(`URL ${index} failed:`, result.reason);
    }
  });
}
```

## Event Loop

Understanding the event loop is crucial for writing performant Node.js code.

```javascript
console.log("1"); // Synchronous

setTimeout(() => {
  console.log("2"); // Macrotask
}, 0);

Promise.resolve().then(() => {
  console.log("3"); // Microtask
});

async function asyncFunc() {
  console.log("4");
  await null;
  console.log("5");
}

asyncFunc();

console.log("6"); // Synchronous

// Output: 1, 4, 6, 3, 5, 2
// Microtasks (Promise.then, async/await) run before macrotasks (setTimeout, setInterval)
```

## Hands-on Exercises

### Exercise 1: Promise Chain
Create a function that:
1. Fetches a user (simulate with setTimeout)
2. Then fetches their posts
3. Then fetches comments for the first post
4. Returns all data

```javascript
// Simulate API calls
function fetchUser(id) {
  return new Promise(resolve => {
    setTimeout(() => resolve({ id, name: "Alice" }), 500);
  });
}

function fetchPosts(userId) {
  return new Promise(resolve => {
    setTimeout(() => resolve([
      { id: 1, title: "Post 1" },
      { id: 2, title: "Post 2" }
    ]), 800);
  });
}

function fetchComments(postId) {
  return new Promise(resolve => {
    setTimeout(() => resolve([
      { id: 1, text: "Great post!" }
    ]), 300);
  });
}

// Solution using async/await
async function getUserData() {
  const user = await fetchUser(1);
  const posts = await fetchPosts(user.id);
  const comments = await fetchComments(posts[0].id);
  return { user, posts, comments };
}
```

### Exercise 2: Async Error Handling
Create a function that tries multiple API endpoints and returns the first successful result:

```javascript
async function tryEndpoints(endpoints) {
  // Your code here - use Promise.any or try/catch with loop
}
```

## Knowledge Check

1. What are the three states of a Promise?
2. When should you use `await` inside a `try/catch`?
3. What runs first: `setTimeout` callbacks or `Promise.then`?
4. How do you handle errors in async/await?
5. What does `Promise.all` do if one promise rejects?

## Next Steps

- [ES6 Features in Depth](./05-es6-features.md)
- [Node.js Introduction](./07-nodejs-introduction.md)
- [Project: Async Data Fetcher](./projects/async-fetcher.md)
