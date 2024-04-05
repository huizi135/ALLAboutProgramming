# Function

## **Write Reusable JavaScript with Functions**

In JavaScript, we can divide up our code into reusable parts called *functions*.

```jsx
function functionName() {
console.log("Hello World");}
functionName();
```

You can call or *invoke* this function by using its name followed by parentheses, like this: `functionName();` Each time the function is called it will print out the message `Hello World` on the dev console. All of the code between the curly braces will be executed every time the function is called.

## **Passing Values to Functions with Arguments**

The actual values that are input (or *"passed"*) into a function when it is called are known as ***arguments***.

Here is a function with two parameters, `param1` and `param2`:

```jsx
function testFun(param1, param2) {
console.log(param1, param2);}
```

```jsx
function functionWithArgs(a, b){
console.log(a + b);}

functionWithArgs(10, 5);
```

output : 15

## **Return a Value from a Function with Return**

We can pass values into a function with *arguments*. You can use a `return` statement to send a value back out of a function.

**Example**

```jsx
function plusThree(num) {
return num + 3;}

const answer = plusThree(5);
```

`answer` has the value `8`.

`plusThree` takes an *argument* for `num` and returns a value equal to `num + 3`.

## **Global Scope and Functions**

In JavaScript, *scope* refers to the visibility of variables. Variables which are defined outside of a function block have *Global* scope. This means, they can be seen everywhere in your JavaScript code.

Variables which are declared without the `let` or `const` keywords are automatically created in the `global` scope. This can create unintended consequences elsewhere in your code or when running a function again. You should always declare your variables with `let` or `const`.

## **Local Scope and Functions**

Variables which are declared within a function, as well as the function parameters, have ***local* scope**. That means they are only visible within that function.

Here is a function `myTest` with a local variable called `loc`.

function myTest() {

const loc = "foo";

console.log(loc);

}

myTest();

console.log(loc);

## **Global vs. Local Scope in Functions**

It is possible to have both *local* and *global* variables with the same name. When you do this, the local variable takes precedence over the global variable.

In this example:

const someVar = "Hat";

function myFun() {

const someVar = "Head";

return someVar;

}

The function `myFun` will return the string `Head` because the local version of the variable is present.

## **Understanding Undefined Value returned from a Function**

A function can include the `return` statement but it does not have to. In the case that the function doesn't have a `return` statement, when you call it, the function processes the inner code but the returned value is `undefined`.

**Example**

let sum = 0;

function addSum(num) {

sum = sum + num;

}

addSum(3);

`addSum` is a function without a `return` statement. The function will change the global `sum` variable but the returned value of the function is `undefined`.

A function can include the `return` statement but it does not have to. In the case that the function doesn't have a `return` statement, when you call it, the function processes the inner code but the returned value is `undefined`.

# **Assignment with a Returned Value**

If you'll recall from our discussion about [Storing Values with the Assignment Operator](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/storing-values-with-the-assignment-operator), everything to the right of the equal sign is resolved before the value is assigned. This means we can take the return value of a function and assign it to a variable.

Assume we have defined a function `sum` which adds two numbers together.

ourSum = sum(5, 12);

Calling the `sum` function with the arguments of `5` and `12` produces a return value of `17`. This return value is assigned to the `ourSum` variable.

// Setup

let processed = 0;

function processArg(num) {

return (num + 3) / 5;

}

// Only change code below this line

processed = processArg(7);

# **Stand in Line**

In Computer Science a *queue* is an abstract *Data Structure* where items are kept in order. New items can be added at the back of the queue and old items are taken off from the front of the queue.

---

Write a function `nextInLine` which takes an array (`arr`) and a number (`item`) as arguments.

Add the number to the end of the array, then remove the first element of the array.

The `nextInLine` function should then return the element that was removed.

function nextInLine(arr, item) {

// Only change code below this line

arr.push(item);

return arr.shift();

// Only change code above this line

}

// Setup

let testArr = [1, 2, 3, 4, 5];

// Display code

console.log("Before: " + JSON.stringify(testArr));

console.log(nextInLine(testArr, 6));

console.log("After: " + JSON.stringify(testArr));

Before: [1,2,3,4,5]

1

After: [2,3,4,5,6]

# **Understanding Boolean Values**

function welcomeToBooleans() {

// Only change code below this line

return true; // Change this line

// Only change code above this line

}

# **Use Conditional Logic with If Statements**

**Pseudocode**

if (*condition is true*) {  *statement is executed*}

**Example**

function test (myCondition) {

if (myCondition) {

return "It was true";

}

return "It was false";

}

test(true);

test(false);
