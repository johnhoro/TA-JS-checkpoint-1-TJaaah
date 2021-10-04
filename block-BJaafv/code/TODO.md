1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}
//here we use return statement  so when we call function it always return value

// second
function sum(a, b) {
  console.log(a + b);
}
```

<!-- // here we doesn't use return statement so it return undefined // -->

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
   the value of first will be same as the value of sum.
   the value of second will be undefined because here we don't use return statement so it gives undefined

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
   it return value 36 because here we use two parameter but when we call the function there is three arguments so function accept only two argument and return the value.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
   Yes we can store first `sum` function in a variable named `add` because function is a object and object is a value and value is an expression so because of that we can store a function in a variable.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

```js
function sayHello(name) {
  return `Hello ${name}`;
}
sayHello(`Arya`);
```

6. What will be the output of the function below and why?

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

showMessage(); //'Hello, John'
```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

alert(userName); // Output 1// john

showMessage(); // Output 2// 'Hello, John'

alert(userName); // Output 3// john
```

8. What is a Anonymous Function give example of three functions.

Anonymous Function is a function that does not have any name associated with it. we use only the function keyword without the function name

```js
let sum = function (a, b) {
  return a + b;
};

let sayHello = function (name) {
  return `Hello ${name}`;
};

let showMessage = function () {
  let message = "Hello, " + userName;
  return message;
};
```

9. Can function declaration be a Anonymous Function? Explain

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
