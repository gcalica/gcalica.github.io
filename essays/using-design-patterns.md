---
layout: essay
type: essay
title: Using Design Patterns
# All dates must be YYYY-MM-DD format!
date: 2018-11-29
labels:
  - Design Patterns
  - Javascript
  - Java
  - Learning
---

# Design Patterns
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Every software engineer has been exposed to a design pattern whether they realize it or not. Of course, software engineers who actually know the existence of design patterns definitely know of this and realize the importance of design patterns. Programmers are exposed to design patterns as soon as they start searching for StackOverflow or Google answers. Or by reading documentation on libraries, frameworks, or any external software they use for their program. This is because those answers and documentation, by nature, give suggestions on how code should be structured based on existing and common design patterns.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Through many years of trial and error, software engineers have found efficient and useful design patterns that they can repeatedly apply through many parts of their program. Implicitly, the way how people structure and write their code is a result of those design patterns being discovered. We will explore some common design patterns that are used in many programs. Specifically, we will explore common design patterns that I have personally used and implemented in a group project that I am working on: [ManoaFixIt](https://github.com/manoafixit/manoafixit)

# ManoaFixIt
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The University of Hawaii at Manoa currently has no fast and minimal effort method of reporting an issue on campus. Specficially, issues that are non-security related. It has a hotline number, but that itself is already counter-productive as no one is gonna bother to remember a campus number that they will barely, if at all, ever use. ManoaFixIt is a web application that me and two other people are building as a group project for a Software Engineering course. Our web application provides a solution to the problem by offering a modern way of submitting issues on campus to the faculty and staff of University of Hawaii at Manoa. And this "modern" solution is done through our web application that is can also be easily used with a smartphone. In order to build our web application, we used many design patterns to help build a solid base for our app to function under.

### Model-View-Controller (MVC)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Model-View-Controller is a very common design pattern found in almost any web application. The 'Model' part of this design pattern is usually our database. It is the part that exposes any functionality of our app and responsible for responding to query calls to the server. It is connected to the 'View' part of our design pattern by notifying any changes to the state of our model to the 'View.' The 'View' is exactly what the word says, it is the part of our app that presents and renders the 'Model.' It is notified by the 'Model' for any changes and requests for the updated changes to render them in 'View.' This 'View' is also connected to our 'Controller' part of the design pattern. The 'Controller' handles and defines the behavior of the functionality of our app. It is connected to 'View' by controlling what 'View' will render and it is connected to 'Model' by updating the 'Model' for any changes in the state.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This design pattern is our top-level pattern that we apply to our web app. In our case, our 'Model' is MongoDB, our 'View' is React, and our Controller is 'React-Router.' In essence, this design pattern also allowed us to organize the work for our web app. Front-end people of our app dealt only with the 'View' and the back-end dealt only with the 'Model' and 'Controller.'

### Singleton
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The Singleton design pattern is a way of creating a single instance of a class, and exposing that instance globally to the rest of the app. This is a way of making sure that we only have one instance of something, and it is only through that instance we invoke the methods of that instance. In our app, this is implemented with our Collections API. We have collection classes that are connected to the MongoDB collection of that collection:
```javascript
class IssuesCollection extends BaseCollection {
  constructor() {
    super('Issues', IssuesSchema);
  }

  ... methods ...
  export const Issues = new IssuesCollection();
}
```
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;As seen from the code above, we implement the Singleton design pattern with the last line of code. We create an instance of IssuesCollection class and expose that instance globally by exporting it. When it comes to MongoDB collections, we only need one instance of a collection to work with. Therefore, this Singleton design pattern is an appropriate design pattern to use for our MongoDB collections. We can then access this collection by defining methods in this Collection class. Since we know that we only have one instance of this collection, we can be confident that any data that we access from this collection has not been touched by another instance.

### Reactive Data


