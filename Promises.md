# Promises

**How to handle errors?:**

1. Asynchronous computation runs: When an asynchronous operation is initiated, such as making an HTTP request or reading a file, it typically runs in the background without blocking the main execution thread. This means that the JavaScript engine can continue executing other code while waiting for the asynchronous operation to complete.

2. Caller is no longer on the stack: In synchronous code, when a function is called, it's added to the call stack, and the JavaScript engine executes it sequentially. However, with asynchronous operations, the function that initiates the asynchronous operation (the caller) may complete and be removed from the call stack before the asynchronous operation finishes.

3. Impossible to throw an exception back to the caller: Since the caller function has already completed and been removed from the call stack by the time the asynchronous operation completes (either successfully or with an error), it's not possible to throw an exception directly back to the caller. This is because the call stack, which would catch the exception, is no longer present.
