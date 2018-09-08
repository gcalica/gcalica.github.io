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

<img class="ui small right circular floated image" src="../images/jslogo.png">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I had been learning and coding with Java for a year, and it is also my first programming language that I have learned. Heading into my third semester as a Comp Sci. major, my ICS 314 (Software Engineering) course uses Javascript instead of Java. After some reading into Javascript, these are my thoughts and worries on Javascript.

# Behavior

### Weakly Typed
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The most immediate difference between Javascript and Java was the declaration of variables. Instead of declaring variables with their explicit type, Javascript simply uses *let* and *const* followed by a variable. That got me immediately thinking, "how do I know what type of variable this is, then?"
  
Instead of having to declare the type of the variable like in Java,
  ```java
  int foo = 0;
  String str = "Hello";
  ```
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I learned that Javascript is what is called a "dynamic typed" and "weakly typed" language. It simply means that Javascript doesn't enforce the correct type. It could care less if you pass just the variable *arr* as an argument into a function, even if that *arr* is supposed to take an array as the argument. 
For example,
```javascript
function test(arr) {
  arr[0] = "Hello World!";
  return arr[0];
}
```
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In the code snippet above, we simply passed *arr* as a parameter for the test function. But if we take a look at what the function is doing, then we can see clearly that *arr* is suppose to be an array based off of the second line. However, it seems like Javascript doesn't seem to care. It just magically seems to know that *arr* is supposed to be a variable that holds an array based on how we inserted the string "Hello World" into the 0*th* index of *arr*. The part that worries me the most when it comes to this "weakly typed" language is that it could possibly be harder to debug code if I don't explicitly know what the type an object is right away. 

### Classes
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Another difference that I learned when it comes to Javascript is that it uses an object-oriented programming style called **prototypal** OO. In Java, there is a distinct difference between a *Class* and an *object*. A Class is the blueprint that creates objects, which are instances of a Class, that contain the object's behavior and states. 
  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;However, in JavaScript, there seems to be no distinct difference between a Class and an object. Classes themselves are also considered objects. There seems to be no real reason to use classes in Javascript other than working with a simpler syntax. 

# Functional Programming
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;One particular thing that I am interested about when it comes to Javascript is functional programming. We all know that Java is an OOP language which means that it primarily uses objects to model real world things. But what if the program that I want to code doesn't need to be modeled after a real world object? In particular, what if I don't want my "objects" and their properties to be constantly changing all over the place. I believe that is when functional programming comes into play. With my limited knowledge of the subject, I think functional programming aims to have *functions* rather than objects as the building blocks for a program. 
  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Rather than modifying the objects themselves, the objects are passed around functions and those functions do the work instead. Functional programming heavily emphasizes on avoiding changing states and working with mutable data. 

***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Overall, I am excited to expand my skillset through learning Javascript. Although Javascript isn't just limited to web development, I have heard that there could be better programming languages than Javascript if I were to use it for non-web development use. Regardless, being able to build a web app through Javascript would be an important skill to have. In the future, I do plan on building websites for my own personal use; therefore, learning Javascript is a good way to start for this future plan.
