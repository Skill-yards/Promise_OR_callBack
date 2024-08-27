

## Task Overview: Working with Callbacks and Promises in JavaScript

### Objective
The goal of this task is to help students understand and practice using callbacks and promises in JavaScript for handling asynchronous operations.

### Task Description
Students will implement functions that simulate fetching user data from a mock API. They will learn to handle asynchronous operations using both callback functions and promises, and explore how to manage errors in both approaches.

### Dummy Data

```javascript
const users = [
    { id: 1, name: "John Doe", email: "john@example.com" },
    { id: 2, name: "Jane Smith", email: "jane@example.com" },
    { id: 3, name: "Alice Johnson", email: "alice@example.com" },
    { id: 4, name: "Bob Brown", email: "bob@example.com" },
    { id: 5, name: "Charlie Davis", email: "charlie@example.com" }
];
```

### Instructions

1. **Create a Mock Data Array:**
   - Use the provided `users` array for the tasks.

2. **Implement a Callback Function:**
   - Write a function that takes an `id` and a `callback` function, simulates a delay using `setTimeout`, and then executes the callback with the corresponding user data or an error message.

3. **Implement a Promise-based Function:**
   - Create a function that returns a promise, which resolves with the user data or rejects with an error message, simulating the delay as before.

4. **Test and Compare:**
   - Test both the callback and promise-based functions with valid and invalid user IDs. Compare how each method handles success and error scenarios.

5. **Optional Challenge:**
   - Combine both approaches in a single function that first attempts to fetch the user with the callback and, if it fails, falls back to the promise.

### Questions

1. **Callback Implementation:**  
   Write a function `fetchUserByIdCallback(id, callback)` that takes an `id` and a `callback` function. The function should simulate a delay using `setTimeout` and execute the callback with either the user data or an error message. Provide an example call to this function with a valid ID.

2. **Error Handling with Callbacks:**  
   How would you modify the `fetchUserByIdCallback` function to handle the case where the user is not found? Write a code snippet that shows how to handle the error within the callback function.

3. **Promise Creation:**  
   Create a function `fetchUserByIdPromise(id)` that returns a promise. The promise should resolve with the user data if found, or reject with an error message if not found. Provide an example of how to call this function using `.then()` and `.catch()`.

4. **Combining Callbacks and Promises:**  
   Suppose you have a function that uses a callback to fetch data but want to use promises for more flexible error handling. How would you combine these approaches in a function that first tries to fetch data using the callback, and if it fails, uses the promise method instead?

5. **Async/Await with Promises:**  
   Convert the `fetchUserByIdPromise` function into an async function and demonstrate how to use `await` to fetch the user data. What are the benefits of using `async/await` over `.then()` and `.catch()`?

