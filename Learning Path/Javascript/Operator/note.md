# **Comparison with the Equality Operator ==**

```jsx
function equalityTest(myVal) {
if (myVal == 10) {
return "Equal";
}
return "Not Equal";
}
1   ==  1  // true
1   ==  2  // false
1   == '1' // true
"3" ==  3  // true
```

# **Comparison with the Strict Equality Operator ===**

Strict equality (`===`) is the counterpart to the equality operator (`==`). However, unlike the equality operator, which attempts to convert both values being compared to a common type, the strict equality operator does not perform a type conversion.

3 ===  3  // true

3 === '3' // false

In the second example, `3` is a `Number` type and `'3'` is a `String` type.

// Setup

```jsx
function testStrict(val) {
if (val === 7) { // Change this line
return "Equal";
}
return "Not Equal";
}
testStrict(10);
```

# **Practice comparing different values**

In the last two challenges, we learned about the equality operator (`==`) and the strict equality operator (`===`). Let's do a quick review and practice using these operators some more.

**Examples**

`3 == '3'` returns `true` because JavaScript performs type conversion from string to number. `3 === '3'` returns `false` because the types are different and type conversion is not performed.

**Note:** In JavaScript, you can determine the type of a variable or a value with the `typeof` operator, as follows:

typeof 3

typeof '3'

`typeof 3` returns the string `number`, and `typeof '3'` returns the string `string`.

// Setup

```jsx
function compareEquality(a, b) {
if (a === b) { // Change this line
return "Equal";
}
return "Not Equal";
}
compareEquality(10, "10");
```

# **Comparison with the Inequality Operator**

1 !=  2    // true

1 != "1"   // false

1 != '1'   // false

1 != true  // false

0 != false // false

**!=** It means "Strictly Equal" and returns **ture**

// Setup

```jsx
function testStrictNotEqual(val) {
if (val != 99) { // Change this line
return "Not Equal";
}
return "Equal";
}
testStrictNotEqual(10);
```

# **Comparison with the Strict Inequality Operator**

**!==** It means "Strictly Not Equal" and returns **`false`**

// Setup

```jsx
function testStrictNotEqual(val) {
if (val !== 17) { // Change this line
return "Not Equal";
}
return "Equal";
}
testStrictNotEqual(10);
```

# **Comparison with the Greater Than Operator >**

`>`) compares the values of two numbers. If the number to the left is greater than the number to the right, it returns `true`. Otherwise, it returns `false`.

```jsx
function testGreaterThan(val) {
if (val > 100) {  // Change this line
return "Over 100";
}
if (val > 10) {  // Change this line
return "Over 10";
}
return "10 or Under";
}
testGreaterThan(10);
```

#
