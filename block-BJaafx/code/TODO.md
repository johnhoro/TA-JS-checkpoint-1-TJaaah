1. Using loops take 10 inputs from user and find the average of all the numbers.

```js
let avg = 0;

for (let i = 1; i <= 10; i++) {
  avg += +prompt(`Enter number for average ${i}`);
}
console.log(avg / 10);
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println("hi");
  i++;
} // println is not defined
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

```js
function getEvenSum(max = 10) {
  let sum = 0;
  for (let i = 1; i <= max; i++) {
    if (i % 2 == 0) {
      sum += i;
    }
  }
  return sum;
}
getEvenSum();
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

```js
function getOddSum(max = 10) {
  let sumOdd = 0;
  for (let i = 1; i <= max; i++) {
    if (i % 2 !== 0) {
      sumOdd += i;
    }
  }
  return sumOdd;
}
getOddSum();
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

```js
function getProductOfDigits(num = `123`) {
  let product = `1`;
  for (let i = 0; i < num.length; i++) {
    product *= num[i];
  }
  return `${product}`;
}
getProductOfDigits();
```

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return "Bigger than 5";
  } else {
    return "Smaller than 5";
  }
  return num;
}

check(10); // "Bigger than 5" // because 10 is bigger than 5 and when we call function it always return value
check(1); // "Smaller than 5"// because 1 is smaller than 5
check(5); // 5 // because 5 is not less than or greater than 5 so it return is 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") return "You are arya";
  if (name === "John") return "You are john";
  return "Who are you";
}

getOutput("Arya"); // `You are arya`// here we use triple equal operator  which check equality and type of value here both are same so it return value
getOutput("John"); // `You are john`// here we use triple equal operator which check equality and type of value here both are same so it return value
getOutput(); // `Who are you` // we just call the function and it  return the value
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") console.log("You are arya");
  if (name === "John") console.log("You are john");
  return "Who are you";
}

getOutput("Arya"); // You are arya // `Who are you`
getOutput("John"); // You are john // `Who are you`
getOutput(); // `Who are you`
```

when we call function it always return value if the function doesn't contain return it will always return undefined

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

```js
function multiReturn(num1 = 2, num2 = 4) {
  return num1 + num2;
  return num1 - num2;
}
multiReturn();// 6 // here multiReturn function contain two return statement when we call the function it return the value of first return and the execution of function will stop
example:-
we have many doors in a room, but we can leave the room from only one door at a time. similarly a function can have multiple return statement but when we call function it return only one return statement at a time.
```

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

we use for loop when we know how many times the loop should run. If we want the loop to break based on a condition other than the number of times it runs, we should use a while loop.
if we have initial value ,ending value and what to do after iteration we use for loop. when we have only condition then we use while loop.

```js
for (let i = 1; i < 10; i++) {
  console.log(i);
}

let i = 1;
while (i < 5) {
  console.log(`hello john ${i}`);
  i++;
}
```
