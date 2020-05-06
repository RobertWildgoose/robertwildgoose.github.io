---
title:  "UK Crime Data"
subtitle: "A C# Library"
author: "Robert Wildgoose"
avatar: "img/authors/robertwildgoose.png"
image: "img/UKCrimeDataC.jpg"
class: "CSharp"
date:   2019-06-22 12:12:12
---
# C# UK Crime Data Library

##Installation

Simply pull this repo down and add the project into your projects solution.
<br>
Once included there are several calls you can make ,which are shown below.

<center><a href="https://github.com/RobertWildgoose/UKCrimeData"><button type="button" class="langbutton">Click Here To View It On Github</button></a></center>

###How do I get a every police force
<pre>var AllPoliceForces = CrimeService.GetAllForces();</pre>

###How do I get a more info on a certain police force ie Wiltshire Police
<pre>var PoliceForce = CrimeService.GetSingleForces("wiltshire");</pre>

###How do I get all crimes for a certain date in a certain location
<pre>var Crimes = CrimeService.GetAllCrimesByPoint("52.9534161", "-1.1492773","2018-10");</pre>
