# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) FUNCTIONS

#### LEARNING OBJECTIVES

*After this lesson, students will be able to:*
- declare a function
- call a function

---

### Intro to functions

Functions help us write cleaner, more organized programs. With a function you can group all the logic specific to a task in one place. The function can then be called when you need to perform that task. This reduces repeating the code in multiple places resulting in smaller programs.

#### Syntax

```javascript
() => {}  // ES6 arrow function
function () {} //pre ES6 function expression

```
#### Assignment

Because a function is a value, data type of `Function Object`, we can assign it to a variable.

```javascript
const countFromTo = () => {
  for(i=1; i<=5; i++) {
    console.log(i);
  }
}
```
---

### Return statement

A function will always return a value even if not explicitly set. Using a `return` statement allows you to specify the value returned. If not set, a function (in most cases) returns `undefined`.



### Calling/Invoking

Invoke a function by placing parentheses, aka, the "call", after the function name.

```javascript
countFromTo(); // 1 2 3 4 5
```

### Parameters and arguments

A function can take in any number of inputs by setting parameters when defining the function. The parameters are variables that can be used in the body of the function.

When we invoke a function, we pass in arguments through the call, the parentheses. Those arguments set the values for the parameters used in the function.

```javascript
const countFromTo = (start, stop) => {
	for (i=start; i<=stop; i++) {
		console.log(i);
	}
	return "Done!";
}

countFromTo(2,7); // 2 3 4 5 6 7 'Done!'
```
---

&#x1F535; **Activity**

Create a function called `getSum` that takes two Number inputs and `returns` the sum of the numbers.

---
### Best practices for functions

- Does one specific thing
- Is self-contained; pass in all values needed
- Name is descriptive action
  - isBlue, getTotal, deleteItem
