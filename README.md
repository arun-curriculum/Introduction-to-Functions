# Introduction to Functions

## Overview

Functions are structures within a variety of programming languages that enable modularity, encapsulation, and reusability in applications. They allow functionality to be set up one time, and then used throughout the application where it is needed.

We will be looking at two different ways to create functions, how we apply them, and lastly some considerations for each methodology respectively.

## Function Declaration

- One of the most common ways you will find functions written is called function "declaration". Declared functions are usually given names. Let's take a simple example:

```javascript
function sayHello() {
	alert("Hello World!");
}
```

- Now that we have declared the function `sayHello`, we can "call" / "run" / "invoke" it to see the output:

```javascript
sayHello();
```

## Dyanamic Functionality

- One of the most important characteristics of functions is that they can change the resulting code behavior based on data that is passed to them.
- The function above is only ever capable of saying "Hello World!". What if we wanted it to be able to say "Hello Arun!" or "Hello Maria!", and more?
- Functions use a combination of **parameters** and **arguments** to make this happen.

### Parameters

- Parameters are data that are set up to work with the intended function.
- An example is a `name` parameter we will use to represent the name that we want to display in the alert:

```javascript
function sayHello(name) { ... }
```

- The `name` here is the parameter, and represents a placeholder for anything we pass to the function when we "call" it.
- Let's try first declaring the function with a name parameter:

```javascript
function sayHello(name) {
	alert("Hello " + name + "!");
}
```

- This function is now capable of saying "Hello {anyone's name}!".

## Arguments

- When you pass data to a function that is expecting a certain parameter, it is called an "argument".
- In the case of our `sayHello` function, the parameter is `name` and the argument is the value for `name` that we provide upon calling the function.
- Let's see an example of this:

```javascript
sayHello("Arun");

sayHello("Maria");
```

- We should now see two alerts - one for Arun and one for Maria.