---
layout: project
type: project
image: images/mfi-logo.png
title: ManoaFixIt
permalink: projects/manoafixit
# All dates must be YYYY-MM-DD format!
date: 2018-11-10
labels:
  - Software Engineering
  - Project Management
  - Meteor
  - React
  - Javascript
  - Web Application Development
summary: Me and my team created a web application called ManoaFixIt that aims to provide UHM community members a modern way to report non-security related issues.
---
# Overview

### Problem
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Currently, University of Hawaii at Manoa (UHM) does not have a quick and modern way to report any non-security related issues that students encounter on campus. There are hotline numbers for students to call, but the process of looking up and finding those numbers is a huge hassle and can even discourage students from reporting issues in the first place.

### Solution
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Our team built a web application called [ManoaFixIt](https://manoafixit.meteorapp.com/#/) to solve this problem which is an app that allows any UHM community member to be able to report any issues they encounter on campus.

### Goals
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;When we built our app, we had two goals in mind:
* Make the web app mobile friendly
* Make it easy to use the app and there should be minimal effort to submit an issue

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Obviously, when students want to report an issue, they would most likely report an issue using their mobile phones. No one is gonna pull out their entire laptop just to submit an issue. Therefore, we built our app to be very mobile friendly and compatible. And since the whole point of the app is to make the process of submitting an issue as less hassle as possible, we also built our app keeping in mind to make it very easy for the user to submit an issue and use our app with minimal effort.

# ManoaFixIt

### Submitting an Issue

<img class="ui image centered" src="../images/manoafixit1.png">
<p align="center"><i> Submitting Issue (Desktop) </i></p>

<img class="ui image centered" src="../images/manoafixit2.png">
<p align="center"><i> Submitting Issue (Mobile) </i></p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This page allows users to submit an issue that they encounter on campus. As you can see, only the Issue Title is required to submit an issue. This is to fulfill our second goal which is to make submitting an issue be very minimal effort.

### List all Issues (Feed Page)

<img class="ui image centered" src="../images/manoafixit3.png">
<p align="center"><i> Feed Page (Desktop) </i></p>

<img class="ui image centered" src="../images/manoafixit4.png">
<p align="center"><i> Feed Page (Mobile) </i></p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This page lists all of the issues that have been submitted. You can search for a particular issue title using the search bar, filter the issues according to a status (Issue Statuses: Open, Accepted, Ongoing, Resolved, and Duplicate), or sort the issues (by Newest, Oldest, Most Liked, and Least Liked). This page only gives you the brief info about that issue: the title, tags, its status, the poster of the issue, how many likes it has, and when the issue was opened. And if you created a particular issue, you can also delete that issue from this page. But if you click on the issue title from this page, it sends you to a page where you can view the full issue's information.

### Individual Issue Pages

<img class="ui image centered" src="../images/manoafixit7.png">
<p align="center"><i> Feed Page (Desktop) </i></p>

<img class="ui image centered" src="../images/manoafixit8.png">
<p align="center"><i> Feed Page (Mobile) </i></p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;After clicking on a particular issue from the Feed page, it redirects you to that issue's individual page. This page gives all the information about the issue: title, description, tags, likes, and its status. From this page, you can click on "Edit Issue" to edit the issue if you were the poster of that issue (as seen from the mobile version picture). Likewise with the Feed page, you can also like the issue from this page. If the logged in user was an Admin account, Admins can change the status of an issue from this page.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Another feature with the issues is that in addition to be able to like an issue, you can also reply to that issue.

### Viewing all Issues on the Map (Map Page)

<img class="ui image centered" src="../images/manoafixit5.png">
<p align="center"><i> Map Page (Desktop) </i></p>

<img class="ui image centered" src="../images/manoafixit6.png">
<p align="center"><i> Map Page (Mobile) </i></p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;When a user submits an issue, the location of where that issue was submitted is tracked. Users can then view all submitted issues whose status Open, Accepted, and Ongoing on the Map page and be able to see the exact location of where an issue was submitted.

# My Contributions

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;For this project, I had two major roles I played: Project Management and Back-End Developer. Our group only had three members--Adrian Au and Graham Francisco on the front-end and me on the back-end. I created the entire back-end for our web application and also helped with the desktop versions of the pages on the front-end side.

### Back-End
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;For our web application, we used the Meteor framework to help build the back-end. Meteor has the built-in MongoDB which we utilized as our database. It was then my job to create the API and the entire structure of our back-end. Thanks to my prior experience with a hackathon where me and another group created a web app, [GATHER](http://gather.meteorapp.com/#/), that was also based off of Meteor, I did not have much trouble learning Meteor unlike my experience with that hackathon. The biggest roadbloack for my back-end development was I have very little experience when it comes to software debugging and testing with Javascript. Like with many Javascript programs, the most common error I encountered was `undefined`. Another framework that we used in conjunction with Meteor was React. When I had to debug certain errors, most documentation and answers I found online used Blaze rather than React, which was another reason why I had trouble debugging some of my code. In order to create the backbone of our back-end, I also utilized and implemented design patterns which I discuss in my essay [Using Design Patterns](https://gcalica.github.io/essays/using-design-patterns.html).

### Front-End
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;We used React as the framework for creating our user interface. React also has a subset of library called React-Router, which we used for routing our back-end. As for my contributions to the Front-End, I contributed to the desktop versions of the Submit, Feed, and Map page while I made the back-end functionality for those pages.

### Project Management
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Out of all the skillsets I utilized and gained, this was the most valuable experience I gained. For our group, I designated myself as the project manager to manage our project. My tasks included managing everything related to our github repository: opening and managing issues, managing the project milestones, doing code reviews, facilitating merge conflicts, and doing pull requests. My job also included facilitating and connecting all back-end code to front-end code. I had the responsibility of making sure that everyone is on the same page as each other and planning which and when steps had to be taken to progress towards our goal of finishing the project.

---
* Deployed Website: [ManoaFixIt](https://manoafixit.meteorapp.com/)
* GitHub Repository: <a href="https://github.com/manoafixit/manoafixit"><i class="large github icon"></i>manoafixit/manoafixit</a>
* GitHub Organization Page: <a href="https://github.com/manoafixit/manoafixit.github.io"><i class="large github alternate icon"></i>ManoaFixIt</a>
* Development Timelapse Video: <a href="https://youtu.be/0p8vGvEfy8M">ManoaFixIt TImelapse</a>



