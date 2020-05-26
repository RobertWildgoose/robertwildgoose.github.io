---
title:  "Random User Generator"
subtitle: "A C# Library"
author: "Robert Wildgoose"
avatar: "img/authors/robertwildgoose.png"
class: "devicon-csharp-plain colored"
image: "img/RandomUserGenerator.jpg"
date:   2019-06-22 12:12:12
---

### What Is It and How Can I Use It
C# Random User Library provides random user data for each call sent out.<br>
Pulling down the code from github and add this to your project.

<a href="https://github.com/RobertWildgoose/RandomUserLib"><button type="button" class="langbutton">Click Here To View It On Github</button></a>

### How do I get a single user?
<pre>var SingleUser = UserGeneratorService.GetSingleUser().results.ElementAtOrDefault(0);</pre>

### How do I get a certain amount of users?
<pre>var MultipleUsers = UserGeneratorService.GetMultipleUsers(10).results;</pre>

### How do I get a previous user back again?
<pre>var MultipleUsers = UserGeneratorService.GetSpecificUser(User.seed).results;</pre>

### How do I get a User from a specific Demographic?
<pre>var SpanishUser = UserGeneratorService.GetSingleUserSpecificNationality(Nationality.Spain).results.ElementAtOrDefault(0);</pre>

### How do I get a Set Of 10 Users from a specific Demographic?
<pre>var MultipleSpanishUser = UserGeneratorService.GetMultiUsersSpecificNationality(Nationality.Spain,10).results;</pre>
