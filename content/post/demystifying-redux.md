+++
date = "2017-06-30T11:10:56+05:30"
author = ""
comments = true
image = "images/redux-2.jpg"
menu = ""
share = true
slug = "demystifying-redux"
categories = [
  "redux",
  "learn redux",
  "pure redux",
  "learn pure redux",
  "vanilla redux",
  "redux js",
  "redux 2015",
  "redux 2016",
  "redux 2017",
  "redux definition",
  "react redux example",
  "redux react tutorial",
  "react redux tutorial 2016",
  "what is redux js",
  "redux tutorial for beginners",
  "proper use of redux",
  "redux usage examples",
  "react redux tutorial 2017"
]
title = "demystifying redux"

+++

![Demystifying Redux](./images/demystifying-redux/home.jpg)

# Introduction

Redux can be complicated at first. 

But after you understand the basics it can be very easy. 

This article will ensure that you understand Redux with the help of some examples. 

After reading this article I promise you, you will say this -

![I know Redux](./images/demystifying-redux/i-know-redux.jpg)

This article will make you fall in love ❤️ with Redux.

According to the [official site](https://redux.js.org/), **Redux** is a predictable state container for JavaScript Applications.

Now what the hell 😕 that means.

Well I'll try to explain it in parts.

# Table of Contents

1. [Why we need Redux?](#why-we-need-redux?)
2. [Immutability](#immutability)
3. [Pure Functions](#pure-functions)
4. [Three Principles of Redux](#three-principles)
    1. [Single Source of Truth](#single-source)
    2. [State is Read Only](#read-only-state)
    3. [Changes are made with pure functions only](#changes-with-pure-functions-only)
5. [Examples](#examples)
    1. [Counter](#counter)
    2. [Todo](#todo)
    3. [Bank](#bank)
6. [Dependants of Redux?](#dependants-of-redux?)
7. [Conclusion](#conclusion)

<a name="why-we-need-redux?"></a>

# 1. Why we need Redux?

Managing State of Application can become cumbersome when the application is a mid-level or enterprise-level application.

That's why we need a mechanism to manage state efficiently so that it can scale to any application from small scale to large scale.

Enter [Redux](https://redux.js.org)

Redux makes it easy to store the state of any application efficiently.

It does that by creating 1 giant object & this giant object consists of all the application state.

Now you might be thinking what the hell is state 😕 !?

State can be anything in the application that needs to be remembered by the application.

For example, 

Consider a simple `COUNTER APPLICATION` which consists of the `CURRENT COUNT` & also has 2 buttons `INCREMENT`  & `DECREMENT`.

![Counter Application](./images/demystifying-redux/counter.png)

Here, the only thing to be remembered in the application is the `CURRENT COUNT` value as it is the one changing constantly whenever user clicks `INCREMENT` or `DECREMENT` button that's why for the `COUNTER APPLICATION`, the state is `CURRENT COUNT`.

Consider another example application like a `BLOG POST`, it will consists of a lot of different blogs.

![Blog Post 1](./images/demystifying-redux/blog-1.png)

Each of the blog post will have `COMMENT` section & each of the comments will have `HEART` to show some love to the post. Here, the state of the application which needs to be remembered is the `COMMENT` & `HEART` as these are the ones changing. 

![Blog Post 2](./images/demystifying-redux/blog-2.png)

`COMMENT` is in the state because if someone clicks on `HEART` to show some love the comment then on which comment it was clicked must be remembered so that's the reason `COMMENT` is needed or if you prefer you can use a specific `ID` which is unique for each comment as the state.

I hope these might have cleared what state really is 😃

<a name="immutability"></a>

# 2. Immutability

Immutability means something that cannot be mutated, i.e, changed or modified after its creation.

Consider an example in JavaScript, 

```
let str = `Hello JavaScript`;
console.log(str.substr(0, 10));
console.log(str);
```

The result of the above code is -

```
Hello Java
Hello JavaScript
```

The `substr()` method on String does not mutate the original string `str`. That's why strings in JavaScript are immutable.

They are not the only immutable value in JavaScript. Numbers are immutable too. 

Numbers example -

```
let x = 10;
x = x + 1;
```

The result of the above code gives value of `x` to be 11.

Now you might be saying how is this immutable !? 😕

The first statement `var x = 10;` assigns value 10 to variable `x`.

The second statement references the `x` to the current value of `x` + 1. 

The statement doesn't change the meaning of value `10`. 

The memory allocated to `x` refers to the new value `11`.

Arrays are mutable in JavaScript.

Consider an example -

```
const arr = [1, 2, 3];
arr.push(4);
console.log(arr);
```

The result of the above code is -

```
[1, 2, 3, 4]
```

This makes sense as Arrays are mutable.

Consider same example using [Immutable JS](https://facebook.github.io/immutable-js/) - 

```
const arr = Immutable.List.of([1, 2, 3]);
arr.push(4);
console.log(arr);
```

The result of the above code is -

```
[1, 2, 3]
```

This is because of Immutability.

Read [Immutable JS](https://facebook.github.io/immutable-js/) docs to learn more about Immutability in JavaScript.

Now why would we use Immutability anywhere !? 🤔

Immutability gives a lot of predictibility.

It means you don't have to check if some array is modified in the code you know it isn't changed by any assignment operator because of its immutable nature.

Example - 

```
const arr = new ImmutableArray([1, 2, 3]); // Imaginary class which creates an Immutable Array
const newArr = arr.push(5);

/*
    ******************************************
    ******************************************
    ******************************************
    ******************************************
    ******************************************
    ******************************************
    ******************************************
    ******************************************
    ******************************************


    some big chunk of code which edits `newArr`


    ******************************************
    ******************************************
    ******************************************
    ******************************************
    ******************************************
    ******************************************
    ******************************************
    ******************************************
    ******************************************
    
*/



console.log(arr); 

/*
 arr is still the same here - [1, 2, 3] 
 if it wasn't immutable it would've changed to the value of newArr
*/

```

This helps in reducing errors & makes us more productive.

It also comes with performance benefits, more times than other.

If you consider Immutability in some parts of operations isolated then the performance will be less.

But if you consider overall performance then it will be a huge benefit.

The following articles are great to know about Immutability in JavaScript - 

[**Immutability in JavaScript**](https://www.sitepoint.com/immutability-javascript/)

[**Immutable Javascript using ES6 and beyond**](https://wecodetheweb.com/2016/02/12/immutable-javascript-using-es6-and-beyond/)

<a name="pure-functions"></a>

# 3. Pure Functions

**Pure Functions** is a functional programming concept.

But, what is a function ? 😕

A function is a process which takes some input & returns some output.

Simple. ❣️

Now, what is a pure function ? 🤔

A function is said to be pure if it returns the same result when given the same parameters.

Consider an example -

```
const square = x => x * x;
square(4); // 16
```

The `square()` function will always return the same value when given the same parameters. 

That's why this function is a pure function.

A more appropriate definition of **Pure Function** is a function which :

* *Given the same input, will always return the same output.*

* *Produces no side effects.*

* *Relies on no external mutable state.*

Example of an **Impure function** is -

```
let count = 0;
const increment = () => count++;
```

The above `increment()` function increments variable `count` outside its own scope. 

The following articles are great to know about Pure Functions in JavaScript - 

[**Master the JavaScript Interview: What is a Pure Function? - By Eric Elliot**](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-pure-function-d1c076bec976)

[**Is your JavaScript Function actually Pure? - By André Staltz**](https://staltz.com/is-your-javascript-function-actually-pure.html)

<a name="three-principles"></a>

# 4. Three Principles of Redux

The part below will sound a little confusing

The 3 basic principles of Redux are - 

<a name="single-source"></a>

## 1. Single Source of Truth

The state of the whole application is stored in a big JavaScript Object.

![Single Source of Truth](./images/demystifying-redux/single-source-of-truth.png)

<a name="read-only-state"></a>

## 2. State is Read Only

State cannot be changed or modified. 

The only way to change state is to emit an action, an object describing what happened.

<a name="changes-with-pure-functions-only"></a>

## 3. Changes are made with pure functions only

Changes are made with pure functions only known as Reducers.

<a name="examples"></a>

# 5. Examples

