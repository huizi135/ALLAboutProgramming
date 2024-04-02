## Variable

```jsx
var ourName;
```

creates a variable called `ourName`. In JavaScript we end statements with semicolons. Variable names can be made up of numbers, letters, and `$` or `_`, but may not contain spaces or start with a number.

## **Assignment operator**

```jsx
var myVar;
myVar = 5;
```

## **Assigning the Value of One Variable to Another**

```jsx
var myVar;
myVar = 5;
var myNum;
myNum = myVar;
```

## **Initializing Variables with the Assignment Operator**

```jsx
var myVar = 0;
```

## **Declare String Variables**

```jsx
var myName = "your name";
```

`"your name"` is called a ***string*** *literal*. A string literal, or string, is a series of zero or more characters enclosed in single or double quotes.

## **Understanding Case Sensitivity in Variables**

```jsx
var someVariable;
var anotherVariableName;
var thisVariableNameIsSoLong;
```

## **Explore Differences Between the** var **and let Keywords**

```jsx
var camper = "James";
var camper = "David";
console.log(camper);
```

In the code above, the `camper` variable is originally declared as `James`, and is then overridden to be `David`. The console then displays the string `David`.

```jsx
let camper = "James";
let camper = "David";
```

The error can be seen in your browser console.

So unlike `var`, when you use `let`, a variable with the same name can only be declared once.

<aside>
💡 **var** can be override declared, but **let** only can be declared once.

</aside>

## **Declare a Read-Only Variable with the const Keyword**

```jsx
const FAV_PET = "Cats";
FAV_PET = "Dogs";
```

<aside>
💡 **constant** value, which means that once a variable is assigned with `const`, it **cannot be reassigned**: **let** can be reassigned and override

</aside>

**uppercase** variable identifiers for **immutable values** and

**lowercase or camelCase** for **mutable values** (objects and arrays)

## **Add Two Numbers with JavaScript**

```jsx
const myVar = 5 + 10;
```

## **Increment a Number with JavaScript**

i++;

is the equivalent of

i = i + 1;

## **Finding a Remainder in JavaScript**

```jsx
var remainder;
remainder = 11 % 3;
```

## **Compound Assignment With Augmented Addition**

```jsx
myVar = myVar + 5;
```

```jsx
let myVar = 1;
myVar += 5;

console.log(myVar);
```

console is 6

# String

## **Escaping Literal Quotes in Strings**

```jsx
const sampleStr = "Alan said, \"Peter is learning JavaScript\".";
```

In JavaScript, you can *escape* a quote from considering it as an end of string quote by placing a *backslash* (`\`) in front of the quote.

This signals to JavaScript that the following quote is not the end of the string, but should instead appear inside the string. So if you were to print this to the console, you would get:

`Alan said, "Peter is learning JavaScript".`

```jsx
var myStr = "I am a \"double quoted\" string inside \"double quotes\"."; // Change this line
```

`I am a "double quoted" string inside "double quotes".`

<aside>
💡 Try to understand how to escape sequence in strings

</aside>

## **Escape Sequences in Strings**

| Code | Output |
| --- | --- |
| \' | single quote |
| \" | double quote |
| \\ | backslash |
| \n | newline |
| \t | tab |
| \r | carriage return |
| \b | backspace |
| \f | form feed |

Test > Assign the following three lines of text into the single variable `myStr` using escape sequences.

`FirstLine`

     `\SecondLine`

`ThirdLine`

```jsx
const myStr = "FirstLine\n\t\\SecondLine\nThirdLine"; // Change this line
```

> `**\\` what is that means, why use `\t`**
> 

## **Concatenating Strings with Plus Operator**

```jsx
const ourStr = "I come first. " + "I come second.";
```

## **Concatenating Strings with the Plus Equals Operator**

```jsx
let ourStr = "I come first. ";
ourStr += "I come second.";
```

## **Constructing Strings with Variables**

```jsx
const ourName = "freeCodeCamp";
const ourStr = "Hello, our name is " + ourName + ", how are you?";
```

`ourStr` would have a value of the string `Hello, our name is freeCodeCamp, how are you?`.

## **Appending Variables to Strings**

```jsx
const anAdjective = "awesome!";
let ourStr = "freeCodeCamp is ";
ourStr += anAdjective;
```

## **Find the Length of a String**

```jsx
// Setup
let lastNameLength = 0;
const lastName = "Lovelace";
// Only change code below this line
lastNameLength = lastName.length;
```

## **Use Bracket Notation to Find the First Character in a String**

```jsx
const firstName = "Charles";
const firstLetter = firstName[0];
```

`firstLetter` would have a value of the string `C`.

## **Understand String Immutability**

In JavaScript, `String` values are *immutable*, which means that they cannot be altered once created.

For example, the following code will produce an error because the letter `B` in the string `Bob` cannot be changed to the letter `J`:

```jsx
let myStr = "Bob";
myStr[0] = "J";
```

Note that this does *not* mean that `myStr` could not be re-assigned. The only way to change `myStr` would be to assign it with a new value, like this:

```jsx
let myStr = "Bob";
myStr = "Job";
```

## **Use Bracket Notation to Find the Nth Character in a String**

```jsx
const firstName = "Ada";
const secondLetterOfFirstName = firstName[1];
```

`secondLetterOfFirstName` would have a value of the string `d`.

## **Use Bracket Notation to Find the Last Character in a String**

```jsx
const firstName = "Ada";
const lastLetter = firstName[firstName.length - 1];
```

`lastLetter` would have a value of the string `a`.

## **Use Bracket Notation to Find the Nth-to-Last Character in a String**

```jsx
const firstName = "Augusta";
const thirdToLastLetter = firstName[firstName.length - 3];
```

`thirdToLastLetter` would have a value of the string `s`.

## **Word Blanks**

Consider this sentence:

It was really ____, and we ____ ourselves ____.

This sentence has three missing pieces- an adjective, a verb and an adverb, and we can add words of our choice to complete it. We can then assign the completed sentence to a variable as follows:

const sentence = "It was really " + "hot" + ", and we " + "laughed" + " ourselves " + "silly" + ".";

const myNoun = "dog";

const myAdjective = "big";

const myVerb = "ran";

const myAdverb = "quickly";

// Only change code below this line

const wordBlanks = "The " + myAdjective + " " + myNoun + " " + myVerb + " " + myAdverb + "."; // Change this line

// Only change code above this line

---

# **ARRAY**

## **Store Multiple Values in one Variable using JavaScript Arrays**

```jsx
const sandwich = ["peanut butter", "jelly", "bread", 3];
```

## **Nest one Array within Another Array**

```jsx
const teams = [["Bulls", 23], ["White Sox", 45]];
```

## **Access Array Data with Indexes**

```jsx
const array = [50, 60, 70];
console.log(array[0]);

const data = array[1];
```

## **Modify Array Data With Indexes**

```jsx
const ourArray = [50, 40, 30];
ourArray[0] = 15;
```

`ourArray` now has the value `[15, 40, 30]`.

<aside>
💡 **Array is changeable, string is not**

</aside>

## **Access Multi-Dimensional Arrays With Indexes**

```jsx
const arr = [[1, 2, 3],
[4, 5, 6],
[7, 8, 9],
[[10, 11, 12], 13, 14]];
const subarray = arr[3];
const nestedSubarray = arr[3][0];
const element = arr[3][0][1];
```

In this example, `subarray` has the value `[[10, 11, 12], 13, 14]`, `nestedSubarray` has the value `[10, 11, 12]`, and `element` has the value `11` .

## **Manipulate Arrays With push Method**

An easy way to append data to the end of an array is via the `push()` function.

`.push()` takes one or more *parameters* and "pushes" them onto the end of the array.

Examples:

```jsx
const arr1 = [1, 2, 3];
arr1.push(4);
const arr2 = ["Stimpson", "J", "cat"];
arr2.push(["happy", "joy"]);
```

`arr1` now has the value `[1, 2, 3, 4]` and `arr2` has the value `["Stimpson", "J", "cat", ["happy", "joy"]]`.

## **Manipulate Arrays With pop Method**

Another way to change the data in an array is with the `.pop()` function.

`.pop()` is used to pop a value off of the end of an array. We can store this popped off value by assigning it to a variable. In other words, `.pop()` **removes the last element** from an array and returns that element.

Any type of entry can be popped off of an array - numbers, strings, even nested arrays.

```jsx
const threeArr = [1, 4, 6];
const oneDown = threeArr.pop();
console.log(oneDown);
console.log(threeArr);
```

The first `console.log` will display the value `6`, and the second will display the value `[1, 4]`.

## **Manipulate Arrays With shift Method**

`pop()` always removes the **last** element of an array. What if you want to remove the **first**?

That's where `.shift()` comes in. It works just like `.pop()`, except it **removes the first element** instead of the last.

Example:

```jsx
const ourArray = ["Stimpson", "J", ["cat"]];
const removedFromOurArray = ourArray.shift();
```

`removedFromOurArray` would have a value of the string `Stimpson`, and `ourArray` would have `["J", ["cat"]]`.

## **Manipulate Arrays With unshift Method**

Not only can you `shift` elements off of the beginning of an array, you can also `unshift` elements to the beginning of an array i.e. add elements in front of the array.

`.unshift()` works exactly like `.push()`, but instead of adding the element at the end of the array, `unshift()` adds the element at the beginning of the array.

Example:

```jsx
const ourArray = ["Stimpson", "J", "cat"];
ourArray.shift();
ourArray.unshift("Happy");
```

After the `shift`, `ourArray` would have the value `["J", "cat"]`. After the `unshift`, `ourArray` would have the value `["Happy", "J", "cat"]`.

| .push() | add the element in the end |
| --- | --- |
| .pop() | removes the last element |
| .shift() | removes the first element  |
| .unshift() | adds the element at the beginning |

## **Shopping List**

const myList = [["bar",4],["juice",1],["cereal",2],["banana",3],["apple",4]];
