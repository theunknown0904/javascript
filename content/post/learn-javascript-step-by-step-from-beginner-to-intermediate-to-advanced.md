+++
date = "2017-06-29T21:39:19+05:30"
author = ""
comments = true
image = ""
menu = ""
share = true
slug = "learn-javascript-step-by-step-from-beginner-to-intermediate-to-advanced"
categories = [
 "javascript",
 "javascript tutorial",
 "javascript tutorials",
 "javascript tuts",
 "javascript download",
 "what is javascript",
 "javascript examples",
 "javascript pdf",
 "javascript free pdf",
 "javascript ebook",
 "javascript free ebook",
 "javascript tutorial pdf",
 "javascript syntax",
 "javascript interview questions and answers",
 "javascript tutorial for beginners",
 "javascript beginner",
 "javascript intermediate",
 "javascript advanced",
 "javascript tutorial with examples",
 "javascript step by step",
 "js",
 "js tutorial",
 "js tutorials",
 "js tuts",
 "js download",
 "what is js",
 "js examples",
 "js pdf",
 "js free pdf",
 "js ebook",
 "js free ebook",
 "js tutorial pdf",
 "js syntax",
 "js interview questions and answers",
 "js tutorial for beginners",
 "js beginner",
 "js intermediate",
 "js advanced",
 "js tutorial with examples",
 "js step by step"
]
title = "learn javascript step by step from beginner to intermediate to advanced"

+++

![So why is JavaScript so good](https://imgur.com/4WqZdpr.png)

# Introduction

This is the most comprehensive guide on Javascript. 

This is not a complete guide as there are 1000 things in Javascript like Type Coercion which are not used 95% of the time. 

So this guide covers everything you need to know about Javascript to write 95% of your code.

# Table of Contents

1. [What is JavaScript](#what-is-javascript?)
2. [Executing JavaScript in Browser](#executing-javaScript-in-browser)
3. [Beginner Level](#beginner-level)
	1. [Numbers](#numbers)
		1. [Data Types](#data-types)
		2. [Integers](#integers)
		3. [Floating Point](#floating-point)
	2. [Basic Arithmetic](#basic-arithmetic)
		1. [Addition](#addition)
		2. [Subtraction](#subtraction)
		3. [Multiplication](#multiplication)
		4. [Division](#division)
		5. [Modulus](#modulus)
	3. [Order of Operations](order-of-operations)	
	4. [Comparators](#comparators)
		1. [Equal To](#equal-to)
		2. [Not Equal To](#not-equal-to)
		3. [Less than](#less-than)
		4. [Greater than](#greater-than)
		5. [Less than or Equal To](#less-than-or-equal-to)
		6. [Greater than or Equal To](#greater-than-or-equal-to)
		7. [Strict Equal](#strict-equal)
		8. [Strict Not Equal](#strict-not-equal)
	5. [Comments](#comments)
		1. [Single Line Comment](#single-line-comment)	
		2. [Multi Line Comment](#multi-line-comment)
	6. [Short Hand Operator](#short-hand-operator)
		1. [Add](#add)	
		2. [Subtract](#sub)
		3. [Multiply](#multiply)
		4. [Divide](#divide)
		5. [Modulus](#mod)	
		6. [Pre-Increment](#pre-increment)	
		7. [Pre-Decrement](#pre-decrement)	
		8. [Post-Increment](#post-increment)	
		9. [Post-Decrement](#post-decrement)	
4. [Intermediate Level](#intermediate-level)
	1. [If...Else](#If-Else)
		1. [if...else](#if-else)
		2. [ternary operator](#ternary-operator)
	2. [do...while](#do-while)	
	3. [while](#while)	
	4. [for-loop](#for-loop)
	5. [switch...case](#switch-case)
	6. [binary and](#binary-and)
	7. [binary or](#binary-or)
	8. [functions](#functions)
	9. [array](#array)
5. [Advanced Level](#advanced-level)
	1. [Immediately Invoked Function Expression (IIFE)](#iife)
	2. [Closure](#closure)
	3. [Hoisting](#hoisting)
	4. [Objects](#objects)
	5. [this keyword](#this)
6. [Conclusion](#conclusion)

<a name="what-is-javascript?"></a>

# 1. What is JavaScript ?

According to Mozilla Developer Network,

> JavaScript is a programming language that allows you to implement complex things on web pages — every time a web page does more than just sit there and display static information for you to look at — displaying timely content updates, or interactive maps, or animated 2D/3D graphics, or scrolling video jukeboxes, etc. — you can bet that JavaScript is probably involved. It is the third layer of the layer cake of standard web technologies, two of which are HTML and CSS.

Simply, JavaScript is nothing but anything that interacts with the user.

For example, clicking a button shows a pop-up ad then that is JavaScript.

Beware, if someone hovers over a button & background color changes then that can be done in both CSS as well as JavaScript.

But, generally CSS is mainly used to provide look & feel of the website & Javascript for the interaction.

<a name="executing-javaScript-in-browser"></a>

# 2. Executing JavaScript in Browser

To run JavaScript open up `Google Chrome` or your preferred Web Browser & open `Developer Tools` then select `Console` Tab. 

Shortcut key for Google Chrome is `F12`.

Then you should see something like the following - 

![Chrome Developer Tools](https://imgur.com/0y9VVZN.png)

<a name="beginner-level"></a>

# 3. Beginner Level

<a name="data-types"></a>

## 3.1. Data Types

Data Types are used to store a particular type of data. The data can be a number, a string or any complex data.

JavaScript has mainly 6 Data Types - object, number, string, boolean, null, & undefined.

JavaScript has Variables.

Variables can be thought of as named containers. You can place data into these containers and then refer to the data simply by naming the container.

Example - 

```
var appleColor = "red";
var age = 18;
// now you can refer `appleColor` & `age`
console.log(appleColor, age); // prints red 18
```

`typeof` gives the data type of the variable.

Examples - 

```
typeof 12 //number
typeof false //boolean
typeof "HELLO WORLD" //string
typeof null //object
typeof undefined //undefined
```

<a name="object"></a>

### 3.1.1. Object

Object is represented as follows - 

```
var john = {
	name: "John",
	age: 40,
	hello: function() {
		return "Hello " + this.name;
	}
};
```

Array is a special type of Object represented as follows - 

```
var arr = [1,2,3,4];
```

Also, Functions is a special type of Object represented as follows - 

```
var hello = function() {
	return "Hello";
};
```

<a name="numbers"></a>

## 3.2. Numbers

JavaScript has integers as well as floating point numbers.

<a name="integers"></a>

### 3.2.1. Integers

Integers are the numbers without decimal point. 

Example - 1, 12, 20, 134, etc.

<a name="floating-point"></a>

### 3.2.2 Floating Point

Floating point numbers are the numbers containing decimal point. 

Floating point numbers are approximated.

Example - 3.1, 12.2, 2.01, 1.34, etc.

<a name="basic-arithmetic"></a>

## 3.3. Basic Arithmetic

JavaScript can perform basic math operations like Addition, Subtraction, Multiplication, Division & Modulus.

<a name="addition"></a>

### 3.3.1. Addition

(1) `12 + 13 = 25`

(2) `2 + 3.5 = 5.5`

(3) `2.5 + 3.5 = 6`

<a name="subtraction"></a>

### 3.3.2. Subtraction 

(1) `17 - 13 = 4`

(2) `17.5 - 4 = 13.5`

(3) `17.3 - 13.1 = 4.200000000000001`

<a name="multiplication"></a>

### 3.3.3. Multiplication

(1) `4 * 12 = 48`

(2) `4 * 6.7 = 26.8`

(3) `4.3 * 6.7 = 28.81`

<a name="division"></a>

### 3.3.4. Division

(1) `12 / 4 = 3`

(2) `9.4 / 4 = 2.35`

(3) `1.4 / 3.4 = 0.4117647058823529`

<a name="modulus"></a>

### 3.3.5. Modulus

(1) `11 % 3 = 2`

(2) `11.3 % 4 = 3.3000000000000007`

(3) `16.78 % 4.5 = 3.280000000000001`

<a name="order-of-operations"></a>

## 3.3. Order of Operations

The Order of Operations in JavaScript is same as that taught in school, i.e, BODMAS

Incase you don't know the abbreviation, BODMAS means Bracket Of Division Multiplication Addition Subtraction

First comes Bracket, i.e, Parentheses have higher precedence then Division & Multiplication have same precedence, i.e, whichever comes first from left to right
then Addition & Subtraction have same precedence, i.e, whichever comes first from left to right

Example - 

(1) `(3 / 2) * 4 = 6`

(2) `3 / (2 * 4) = 0.375`

(3) `3 / 2 * 4 = 6`

(4) `3 * 2 / 4 = 1.5`

(5) `3 + 2 - 1 = 4`

(6) `3 - 1 + 2 = 4`

(7) `(6 + 7) * 5 / 6 + 3 - 2 * 5 / 3 = 10.5`

(8) `2 + (6 % (2 + 1)) = 2`

(9) `(-8 * 16) - 9 * -3 = -101`

<a name="comparators"></a>

## 3.4. Comparators

<a name="equal-to"></a>

### 3.4.1. Equal To

(1) `4 == 2` returns `false`

(2) `2 == 2` returns `true`

(3) `'2' == 2` returns `true`

<a name="not-equal-to"></a>

### 3.4.2. Not Equal To

(1) `4 != 2` returns `true`

(2) `2 != 2` returns `false`

(3) `'2' != 2` returns `false`

<a name="less-than"></a>

### 3.4.3. Less than

(1) `4 < 2` returns `false`

(2) `2 < 3` returns `true`

(3) `'2' < 3` returns `true`

<a name="greater-than"></a>

### 3.4.4. Greater than

(1) `4 > 2` returns `true`

(2) `2 > 3` returns `false`

(3) `'2' > 3` returns `false`

<a name="less-than-or-equal-to"></a>

### 3.4.5. Less than or Equal To

(1) `4 <= 2` returns `false`

(2) `2 <= 3` returns `true`

(3) `'2' <= 3` returns `true`

<a name="greater-than-or-equal-to"></a>

### 3.4.6. Greater than or Equal To

(1) `4 >= 2` returns `true`

(2) `2 >= 3` returns `false`

(3) `'2' >= 3` returns `false`

<a name="strict-equal"></a>

### 3.4.7. Strict Equal

(1) `4 === 2` returns `false`

(2) `2 === 2` returns `true`

(3) `'2' === 2` returns `false`

<a name="not-equal-to"></a>

### 3.4.8. Not Equal To

(1) `4 !== 2` returns `true`

(2) `2 !== 2` returns `false`

(3) `'2' !== 2` returns `true`

<a name="comments"></a>

## 3.5. Comments

<a name="single-line-comment"></a>

### 3.5.1. Single Line Comment

Single Line Comments are displayed by `//`

Example - 

`// this is a single line comment`

<a name="multi-line-comment"></a>

### 3.5.1. Multi Line Comment

Multi Line Comments are displayed by putting comment between `/*` & `*/`

Example - 

```
/* 
this is a multi line comment
*/
```

<a name="short-hand-operator"></a>

### 3.6. Short Hand Operator

Short Hand Operators are used to reduce syntax.

<a name="add"></a>

### 3.6.1. Add

Represented by `+=`

Example - 

```
var a = 1;
a += 2; // 3
```

<a name="sub"></a>

### 3.6.2. Subtract

Represented by `-=`

Example - 

```
var a = 3;
a -= 2; // 1
```

<a name="multiply"></a>

### 3.6.3. Multiply

Represented by `*=`

Example - 

```
var a = 3;
a *= 2; // 6
```

<a name="divide"></a>

### 3.6.4. Divide

Represented by `/=`

Example - 

```
var a = 3;
a /= 2; // 1.5
```

<a name="mod"></a>

### 3.6.5. Modulus

Represented by `%=`

Example - 

```
var a = 3;
a %= 2; // 1
```

<a name="pre-increment"></a>

### 3.6.6. Pre-Increment

Represented by `++a`

It increments the variable first then returns the value

Example - 

```
var a = 3;
console.log(++a); // 4
```

<a name="pre-decrement"></a>

### 3.6.7. Pre-Decrement

Represented by `--a`

It decrements the variable first then returns the value

Example - 

```
var a = 3;
console.log(--a); // 2
```

<a name="post-increment"></a>

### 3.6.8. Post-Increment

Represented by `a++`

It returns the variable first then increments its value

Example - 

```
var a = 3;
console.log(a++); // 3
// now a = 4
```

<a name="post-decrement"></a>

### 3.6.9. Post-Decrement

Represented by `a--`

It returns the variable first then decrements its value

Example - 

```
var a = 3;
console.log(a--); // 3
// now a = 2
```
<a name="intermediate-level"></a>

# 4. Intermediate Level

<a name="If-Else"></a>

# 4.1. If...Else

If...Else statements are executed on certain condition

The main gist of If...Else is if some condition is true then perform X otherwise perform Y

Following are the 2 ways to write If...Else statements - 

<a name="if-else"></a>

# 4.1.1. if...else

if...else in JavaScript is represented as follows - 

```
if(/* some condition*/) {
	/* perform this if condition is true */
}
else {
	/* perform this if condition is false */
}
```

We can also have nested if...else represented as follows -

```
if(/* some condition*/) {
	if(/* some other condition*/) {
		/* perform this if both conditions are true */
	}
	else {
		/* perform this if 1st condition is true & 2nd condition is false */
	}
}
else {
	/* perform this if condition is false */
}
```

We can also have if...else...if represented as follows - 

```
if(/* some condition*/) {
	/* perform this if condition is true */
}
else if(/* some other condition*/) {
	/* perform this if 1st condition is false & 2nd condition is true */
}
else {
	/* perform this if both conditions are false */
}
```

<a name="ternary-operator"></a>

# 4.1.2. ternary operator

ternary operator is represented by `? :`

Example - 

```
var even = x % 2 === 0 ? true : false;
```

If `x % 2 is 0` then `even` is set to `true` else it is set to `false`

<a name="do-while"></a>

# 4.2. do...while

do while loop is also known as exit controlled loop since the condition is checked when exiting the loop

```
do {
	/*
		some code
	*/
} while(/* some condition*/);
```

Example - 

```
var x = 4;
do {
	x /= 2;
} while(x % 2 != 1);
```

<a name="while"></a>

# 4.3. while

while loop is also known as entry controlled loop since the condition is checked when entering the loop

```
while(/* some condition*/) {
	/*
		some code
	*/
};
```

Example - 

```
var x = 4;
while (x/2 !== 0) {
	x--;
};
```

<a name="for-loop"></a>

# 4.4. for-loop

for loop is used when number of iterations to be performed are already known

```
for(/* initialization */ ; /* some condition*/ ; /* modification */) {
	/*
		some code
	*/
};
```

Example - 

```
for(var i = 0; i < 5; i++) {
	console.log(i);
}
```

<a name="switch-case"></a>

# 4.5. switch...case

switch case is used when there are multiple if...else's

Example - 

```
var x = 'A';
switch(x) {
	case 'a':
	case 'A':
	case 'e':
	case 'E':
	case 'i':
	case 'I':
	case 'o':
	case 'O':
	case 'u':
	case 'U':
		console.log('Vowel');
		break;
	default: 
		console.log('Consonant');
};
```

<a name="binary-and"></a>

# 4.6. binary and

`binary and` is represented by `&&`

```
true && true = true
false && true = false
true && false = false
false && false = false
```

Example - 

```
var a = true;
var b = false;
var c = a && b;
console.log(c); // false
```

<a name="binary-or"></a>

# 4.7. binary or

`binary or` is represented by `||`

```
true || true = true
false || true = true
true || false = true
false || false = false
```

Example - 

```
var a = true;
var b = false;
var c = a || b;
console.log(c); // true
```

<a name="functions"></a>

# 4.8. functions

Functions are used when some chunk of code is repeated more than once 

Example - 

```
// Function Declaration
function isOdd(x) {
	return x % 2 === 1;
}

// Function Call
isOdd(5); // true
```

Functions can be stored in a variable for later use

```
var oddFn = function isOdd(x) {
	return x % 2 === 1;
};

oddFn(4); // false
```

Functions can also be anonymous when stored in a variable

```
var oddFn = function(x) {
	return x % 2 === 1;
};

oddFn(1); // true
```

<a name="array"></a>

# 4.9. array

Arrays are special types of objects which have keys as the numbers starting from index `0`

Arrays are declared as follows - 

```
var arr = [1, 2, 3, 4, 5];
```

There are different methods on array such as `length`, `push()` , `pop()`, `shift()` & `unshift()`

All methods can be found by console logging `Array().__proto__`

Example - 

```
var arr = [1, 2, 3];
arr.length; // 3
arr.push(4); // [1, 2, 3, 4]
arr.pop(); // [1, 2, 3]
arr.unshift(4); // [4, 1, 2, 3]
arr.shift(); // [1, 2, 3]
```

<a name="advanced-level"></a>

# 5. Advanced Level

<a name="iffe"></a>

# 5.1. Immediately Invoked Function Expression (IIFE)

IIFEs are used inorder not to bloat the global namespace

IIFE stands for Immediately Invoked Function Expression which means the function gets called immediately after declaration

It is represented as follows - 

```
(function () {
	console.log('I am an IFFE');
})();
```

<a name="closure"></a>

# 5.2. Closure

Closure is an inner function who has access to the outer functions variables

Example - 

```
function outer(name, age) {
	
	function inner() {
		console.log('My name is ' + name + ' & my age is ' + age);
	}

	return inner;
}


var john = outer('John', 38);
john(); // My name is John & my age is 38
```

Notice that the variables `name` & `age` are still remembered long after the function is executed

The variables `name` & `age` are global to the `inner` function

Another example of Closure can be as follows -

```
var updateFn = function() {
	var counter = 0;
	return function() {
		return ++counter;
	};
};
var updateCounter = updateFn();
updateCounter();
```

The variable `counter` is freed from the memory as soon as `updateFn` is executed but it is because of `Closure` that the value of `counter` is still remembered

<a name="hoisting"></a>

# 5.3. Hoisting

Hoisting in JavaScript moves the declaration of variables & functions to the top

JavaScript Declarations are hoisted

Example - 

```
// What we write
function add() {
	var add2Numbers = sum(5,6);
	return add2Numbers;

	function sum(x, y) {
		return x + y;
	}
}


// How JavaScript sees
function add() {
	var add2Numbers = undefined;
	function sum(x, y) {
		return x + y;
	}

	add2Numbers = sum(5,6);
	return add2Numbers;
}
``` 

Also, in JavaScript Hoisting, functions are hoisted first, then variable declarations

Example - 

```
function a() {}
var a;
console.log(a); // function a() {}
```

As variable `a` is undefined; `function a() {}` will be logged

Another Example - 

```
var a;
function a() {}
console.log(a); // function a() {}
```

Here, also it logs out `function a() {}`

<a name="objects"></a>

# 5.4. Objects

In JavaScript, everything is an Object

All JavaScript values except Primitive Values are Objects

Primitive Values are `null`, `undefined`, `boolean`, `string` & `number`

Objects are Data Types containing `<key, value>` pair

Example - 

```
var person = {
	name: 'Desmond Hume',
	age: 43,
	quote: 'I will see you in another life, brotha'
};
```

In the above example, `person` is an object

The `<key>` in the `<key, value>` pair must always be a string & the `<value>` can be any Data Type in JavaScript even another Object

Example - 

```
var person = {
	name: {
		firstname: 'Desmond',
		lastname: 'Hume'
	},
	age: 43,
	quote: 'I will see you in another life, brotha'
};
```

The `<value>` can also be a function

Example - 

```
var person = {
	name: {
		firstname: 'Desmond',
		lastname: 'Hume'
	},
	age: 43,
	quote: 'I will see you in another life, brotha',
	printAge: function() {
		console.log(this.age);
	}	
};
```

Objects can also be created using the `new` keyword

Example -

```
var person = new Object();
person.name = 'Desmond Hume';
person.age = 43;
```

The above method creates only one object

Inorder to create Multiple Objects we need to use Object Constructor

Example - 

```
function movie(name, rating, year) {
	this.name = name;
	this.rating = rating;
	this.year = year;
}

var TheGodfather = movie('The Godfather', 9.5, 1972);
var Drishyam = movie('Drishyam', 8.8, 2016);
```

By using the Object Constructor method we can create Multiple Objects

<a name="this"></a>

# 5.5. `this` keyword

As seen in the example above, `this` keyword is used

Notice that `this` is not a variable in JavaScript, it is a keyword which means you cannot change the value of `this`

The value of `this`, when used in a function, is the object that owns the function

The value of `this`, when used in an object, is the object itself

The `this` keyword in an object constructor does not have a value. It is only a substitute for the new object. The value of `this` will become the new object when the constructor is used to create an object.

Example - 

```
function tvseries(name, year) {
	this.name = name;
	this.year = year;
}

var Lost = tvseries('Lost', 2004);
var Dexter = tvseries('Dexter', 2006);
var GOT = tvseries('GOT', 2011);
```

Here is another example of `this` -

```
var person = {
	name: 'Joey',
	printName: function() {
		console.log(this.name);
	}
};

person.printName(); // Joey
```

<a name="conclusion"></a>

# 6. Conclusion

I hope by now you have learnt 95% of the JavaScript we require to write clean & efficient code.

Now you can go ahead & start coding. 😃

If you want to dive deeper into JavaScript here are some recommended books order wise. 

Awesome ❤️ books appear at the top.

[You Don't Know JS](https://www.amazon.com/You-Dont-Know-Js-Book/dp/B01AY9P0P6)

