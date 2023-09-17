---
title: "Simplest example of  Callbacks  in JavaScript"
datePublished: Tue Sep 12 2023 05:53:38 GMT+0000 (Coordinated Universal Time)
cuid: clmfwdb47000608jzc9zk7wsh
slug: simplest-example-of-callbacks-in-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1694497956506/d9ba99ce-3b5b-43ba-b7f4-eb925a11a0d7.jpeg
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1694497934345/06383657-bc3b-48de-b199-64bb236b3e1b.jpeg
tags: code, javascript, functional-programming, callback, example

---

### First of all, **what is Callback in JS?**

A callback is a function that's passed as an argument to another function and is executed once that function has completed its task. Callbacks are commonly used to handle asynchronous operations like fetching data from an API, reading files, or executing timed events.

**Example: Add and Divide two numbers using a callback function**

Let's dive into a simple example to grasp the concept of callbacks. We have two basic operations, addition and division, and we want to perform these operations using callback functions. Here's how it works:

```javascript
function add(a, b) {
  return a + b;
}

function divide(a, b) {
  return a / b;
}

function calculate(x, y, operationCallback) {
  const result = operationCallback(x, y);
  return result;
}

function callbackExample() {
  const sum = calculate(2, 2, add);
  const quotient = calculate(6, 2, divide);
  console.log(`Sum: ${sum}`);
  console.log(`Quotient: ${quotient}`);
}

callbackExample();
```

* We define two basic operations, `add` and `divide`, which takes two numbers and returns their respective results.
    
* The `calculate` function accepts two numbers (`x` and `y`) and a callback function (`operationCallback`). It invokes the callback function with the provided numbers and returns the result.
    
* We use the `calculate` function with callbacks to perform addition and division, resulting in the variables `sum` and `quotient`.
    
* Finally, we log the results to the console.
    

*Thanks for exploring the world of JavaScript callbacks with us. Keep coding, keep learning, and remember, JavaScript is a boundless journey of discovery. Share this blog with others if you found it helpful.*

*Happy coding!*