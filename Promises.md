# Promises


   
:question: **What is a promise?** 
Promises are just a different way of working with callbacks. Since async programming breaks exception handling, promises help standardize a way to handle errors. They provide a way for errors to propagate correctily thru a chain of promises. 

**If a problem is fulfilled:** The value is a return value that gets passed to any callbuck functions registered as the first argument of then.
**If a promise is rejected:** The value is an error of some sort that is passed to any callback functions registered with catch. 


:question: **What is .then()?**
Instead of nested callback functions which can be unwieldy, functions are defined in a nested then() method in a linear promise chain.
when the promise returns a value, you usually want to do something with that value. 
They act like a callback registration like the addEventListener() method that is used for registering event handlers in client-side JavaScript. ALtho unlike event listeners a Promise represents a single computation. Each function with .then() will only be invoked once. The computation is performed after the promise object is returned to us. 


:question: **How to handle errors?**

1. Asynchronous computation runs: When an asynchronous operation is initiated, such as making an HTTP request or reading a file, it typically runs in the background without blocking the main execution thread. This means that the JavaScript engine can continue executing other code while waiting for the asynchronous operation to complete.

2. Caller is no longer on the stack: In synchronous code, when a function is called, it's added to the call stack, and the JavaScript engine executes it sequentially. However, with asynchronous operations, the function that initiates the asynchronous operation (the caller) may complete and be removed from the call stack before the asynchronous operation finishes.

3. Impossible to throw an exception back to the caller: Since the caller function has already completed and been removed from the call stack by the time the asynchronous operation completes (either successfully or with an error), it's not possible to throw an exception directly back to the caller. This is because the call stack, which would catch the exception, is no longer present.
   
