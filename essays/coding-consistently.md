---
layout: essay
type: essay
title: Coding Consistently
# All dates must be YYYY-MM-DD format!
date: 2018-09-19
labels:
  - Coding Standards
  - IntelliJ
  - ESLint 
  - Javascript
  - Learning
---
# Coding Standards
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Using coding standards or conventions is a standard software engineering process to improve overall readability and structural quality of your code. But why follow them? Considering the fact that they are not really enforced by compilers. Maybe your favorite IDE could conform to basic coding standards by formatting it for you (provided that you actually command the IDE to format your code), but that approach is quite limited. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Coding standards are more than just how many spaces each line of code should indent or how many whitespaces should be between each function or method. They can also include naming conventions for your file, function, or variable names. Since there are many ways to code a certain program or function, coding standards also sets the baseline as to how these programs or functions are supposed to look like syntactically. 

###Productivity
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Backed by many studies, it has been proven that most of your time spent 'programming' is actually debugging. Debugging means that you have to go through and read possibly thousands or more lines of code. If each person or a few people in the development team do not follow the coding standard defined by the team, it significantly decreases productivity. This is especially the case when you are reading someone else's code with a different coding format than that set by the standard of your team. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;When you have a consistent coding standard, reading code becomes much easier as you do not have to look too much into someone else's code to know where and how things are happening. For example,
```javascript
function functionChain(data) {
  return _.chain(data).filter(key => key > 2).uniq('ID').reduce((memo, key) => memo + key).value(); 
}
```
From the code snippet above, we cannot easily pick up what this function may be doing. However, if we had set a coding standard where you are required to start a new line for each function call in any function chain:
```javascript
function functionChain(data) {
  return _.chain(data)
  .filter(key => key > 2)
  .uniq('ID')
  .reduce((memo, key) => memo + key)
  .value(); 
}
```
Now we can more clearly read and see what exactly is happening in the function above. 

#Linters
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;As coding standards have become a highly recommended practice in development in general, people have created many tools to better enforce these coding standards and remind you of any errors that go against the coding standards. Some of these tools are called linters. Linter(s) is a tool(s) that analyzes your code to flag any programming errors, bugs, and any stylistic errors that could go against the coding standard you have setup for your program. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;From my own personal experience, linters have increased the quality of my code. I'm currently programming in Javascript using EMCAScript 6, and the use of a linter called ESLint have reminded me of the many uses and features that come with EMCAScript 6. For example, the use of template literals. Coming from Java, I was used to Java's concatenation of strings--- ``` String c = String a + String b + "Some text";``` However, ESLint has constantly reminded me over and over to use template literals for a better formation option that utilizes ES6. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;It has also taught me more on what it actually means for something to be *const*. I used to declare arrays with *let* rather than *const*. I figured that adding to the array would make it 'non-constant.' It wasn't until ESLint pointed out that I should be using *const* for declaring most of my arrays that I learned that a *const* object can have its properties mutated. This discovery has led me to read more on immutable and mutable objects. 
