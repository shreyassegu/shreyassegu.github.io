---
layout: post
title:  "Quick Javascript notes"
categories: [ Javascript, Tutorials, ES6 ]
image: https://images.unsplash.com/photo-1517842645767-c639042777db?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1280&q=60 
beforetoc: "Quick and simple, easy to understand javascript ES6 notes for reference"
featured: true
toc: true
comments: false
---

## var

The OG variable in Javascript which has some weird quirks, like being able to use a variable without actually declaring it, hoisting of these variables which added more to the confusion, no block scoping, etc.

Now with ES6 we can think of var as a variable which has global scope, but I don't recommend using it always when we have another option which makes more sense.
Some weird examples...


```js
message = “Hello world”
console.log(message)
var Message;
```

```js
if(true){
    bar message = “Hello world”
}
console.log(message)
```
[MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var)

## let

This is a new syntax which was introduced in ES6 and fixes some of the problems which the old variable had.
- Does not get hoisted
- Block scoped
- Cannot be used before declaration
This allows the variable to have expected and predictable behavior, allows developers to write clean and easy to debug code

```js
let message = “one”;
if(true){
    Let message = “two”;
    console.log(message); //two
}
console.log(message); //one
```
[MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let)

## const

As the name implies, this is used to declare a constant variable. Once initialized it cannot be re-initialized, a common practice is to name the variables in full capital casing to indicate that they are indeed constants.

```js
const a = 10;
a = 20;
//error
```
An important thing to keep in mind about constants are the reference types which you assign, such as arrays and objects. These values can be altered as the reference to the objects are not being changed, only the value is

```js
const arr = [10,20,30];
arr.push(40);
console.log(arr); //10,20,30,40
```

```js
const person = {
    name : "abc"
};
person.name = "xyz";
console.log(person.name); //xyz
```

## Fat Arrow Functions

An arrow function is a new syntax for writing functions, lets compare the old way and the new way for writing a function, this syntax makes writing functions inside callbacks smaller, and more readable

```js
//old
function helloWorld(){
    return "Hello world!";
}
console.log(helloWorld()); //Hello world!
```
```js
//new
let helloWorld = () => "Hello world!";
console.log(helloWorld()); //Hello world!
```

- If you are not passing any arguments to the arrow function, you need to have the empty pair of parenthesis
- If you are passing only one argument, no need for parenthesis
- If there is only one statement, you don't need to use return statement

## "**this**" keyword in arrow functions

The keyword "this" in normal functions always keeps changing context depending on where it is being called.

The same "this" in arrow functions retain the context from where it is declared, rather from where it is being called, this is the most important functionality to remember and keep in mind when working with JS

## Default function parameters

Function parameters can be assigned a default value 
todo