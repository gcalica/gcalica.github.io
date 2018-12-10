---
layout: project
type: project
image: images/gather.png
title: HACC 2018: GATHER App
permalink: projects/gather
# All dates must be YYYY-MM-DD format!
date: 2018-11-10
labels:
  - Hackathon
  - HACC 2018
  - GATHER
  - Software Engineering
  - Web Development
  - Backend Development
summary: I participated in my first hackathon, the Hawaii Annual Code Challenge 2018, and created the GATHER app with six other members.
---

# Overview
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;On October 20, 2018, coders of all levels, from amateurs to working professionals, gathered around in the East-West Center on the University of Hawaii campus to attend the Hawaii Annual Code Challenge (HACC 2018). This year's theme for the hackathon was centered around the sustainability goals presented by the [Aloha Challenge Dashboard](https://dashboard.hawaii.gov/aloha-challenge). During the kickoff event, a total of seven different departments presented challenges that each department is facing and need help in. The challenge that my group decided to take on was the Office of Sustainability (UH)'s challenge on Waste Audit Data Collection.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;University of Hawaii's Office of Sustainability is working to help the University of Hawaii(UH) campus to move towards a goal of a zero-waste policy. In order to figure out which areas the UH campus needs to improve in, the Office of Sustainability conducts Waste Audit events that are designed to observe and track the waste stream of the campuses. The Waste Audits provide valuable data to UH to help in making decisions to move towards the zero-waste policy.

# Waste Audit
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Typically, one Waste Audit event relates to one of the UH campuses and several buildings of that campus. Of the several selected buildings for the Waste Audit event, the trash from each building is collected and sorted into different categories. These categories include paper, glass, metal, and plastic materials. The trash are sorted into trash bags based on their category and recorded. The weight and volume of each trash bag is recorded, which is the main data for the event.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The Waste Audit also encourages and invites students, community members, and volunteers as its workers for the event. This creates a positive environment of a group of people who are like-minded towards the goal of achieving a zero-waste policy for the campuses.

### Problem
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Currently, data collection during the Waste Audit event is very inefficient. As it is, data collection for the Waste Audit is actually just pencil and paper, which can get pretty messy as trash is handled all over the place and sticky things can get onto the paper. Not only that, sorting the data is also very tedious and inefficient. After all the data has been recorded, the maintainer of the data has to input each data one by one into a spreadsheet. And then they also have to make the charts to visualize these data themselves.

### Solution
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The problems can be solved by streamlining the Waste Audit data collection into a much more efficient and modern process. Our group provided a solution for this problem by creating a web application that did almost all of the work that the maintainer of the data collection had to do. We also created hardware to solve the part of the process where the Waste Audit volunteers had to record the data for each trash bag collected had been solved.

# GATHER

Our solution consisted of two parts:
* Hardware: the Smart Bin.
* Software: Our web application [GATHER](http://gather.meteorapp.com/#/)

### Smart Bin
<img class="ui image circular centered" src="../images/trashbin.jpg">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;With the old process of data collection, the Waste Audit volunteers had to write down the data for each trash bag. This included the respective category, weight, and volume for that trash bag. To solve this problem, a member of our team created a smart trash bin that could sense the weight and track the items that go inside the trash bin. The tracked data from the bin would then be sent over to the servers of our web application to be recorded and saved in the database. This contraption can also be expanded so that these trash bins can be placed all over campus, and students can actually sort and throw their trash into these bins to help contribute to the data collection.

### Web App
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Besides the trash bin, there is also a manual process of recording the data from the Waste Audit into our web app.

<img class="ui image centered" src="../images/gatherapp1.png">

In this page of our web application, the Waste Audit volunteers can manually enter the data for each trash bag that was sorted. This is a much more efficient process than the old pencil and paper as all data can be found in one centralized database--our web app.

<img class="ui image centered" src="../images/gatherapp2.png">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

# My Contribution
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I was assigned as one of the two back-end developers, responsible for creating the back-end structure of our web app. My tasks included creating the API of our web application, setting up our MongoDB database in mLab, and creating the collections ("tables" is the equivalent in SQL language) of our database. And the majority of my contributions were the Wrapper class on the server-side. The Wrapper class is a class of modules to be used by our front-end developers. The functions inside the Wrapper class all connect to our MongoDB database, and their primary function is to query and fetch data from the database. Our back-end was composed of many collections, therefore it was my job was to be able to query those data. These functions would then be used by our front-end programmers to render the data back into our web application.

---
* Deployed Website: [GATHER](http://gather.meteorapp.com/#/)
* GitHub Repository: <a href="https://github.com/HACC2018/The-Johnson-Family"><i class="large github icon"></i>HACC2018/The-Johnson-Family</a>



