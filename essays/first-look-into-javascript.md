---
layout: essay
type: essay
title: First look into JavaScript
# All dates must be YYYY-MM-DD format!
date: 2018-08-31
labels:
  - JavaScript
  - Learning
---

##Syntax
  There were a few immediate differences that I noticed when I first started reading into Javascript between JS and Java. I had been learning and coding with Java for a year, and it is also my first programming language that I have learned. I was already getting comfortable with Java, especially with inheritance in an object-oriented programming language. The most obvious difference between JS and Java was the syntax. Instead of declaring variables with their primitives, Javascript simply uses "let" and "const" followed by a variable. That got me immediately thinking, "how do I know what type of variable this is, then?"
  
Instead of having to declare the type of the variable like in Java,
  ```java
  int foo = 0;
  String str = "Hello";
  ```
I learned that Javascript is what is called a "dynamic typed" and "weakly typed" language. It simply means that Javascript doesn't enforce the correct type. It could care less if you pass just the variable "arr" as an argument into a function, even if that "arr" is supposed to take an array as the argument. 
For example,
```javascript
function test(arr) {
  arr[0] = "Hello World!";
}
```
In the code snippet above, we simply passed "arr" as an argument for the test function. But if we take a look at what the function is doing, then we can see clearly that "arr" is suppose to be an array. However, it seems like that Javascript doesn't seem to care. It just magically seems to know that arr is a function based on how we inserted the string "Hello World" into the 0th index of arr. The part that worries me the most when it comes to this "weakly typed" language is that it could possibly be harder to debug code if I don't explicitly know what the type an object is right away. 

##Functional Programming
One particular thing that I am interested about when it comes to Javascript is functional programming. We all know that Java is an OOP language which means that it uses objects to model real world things. But what if the program that I want to code doesn't need to be modeled after a real world object? In particular, what if I don't want my "objects" and their properties to be constantly changing all over the place. I believe that is when functional programming comes into play. With my limited knowledge of the subject, I think functional programming aims to have *functions* rather than objects as the building blocks for a program. Rather than modifying the objects themselves, the objects are passed around functions and those functions do the work instead.

