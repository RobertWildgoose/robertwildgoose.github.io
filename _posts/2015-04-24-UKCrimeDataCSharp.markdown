---
title:  "UK Crime Data"
layout: post
subtitle: "A C# Library"
author: "Robert Wildgoose"
avatar: "img/authors/robertwildgoose.png"
image: "img/projects/UKCrimeDataC.jpg"
class: "devicon-csharp-plain colored"
date:   2019-11-11 12:12:12
link: https://github.com/RobertWildgoose/UKCrimeData
type: DevelopmentLibrary
---
<div class="post-heading">
	<div class="post-image-container">
		<img class="project-logo" src="{{ site.baseurl }}/img/projects/UKCrimeDataC.jpg"/>
	</div>
	<div class="post-bio-container">
		<h2>Installation</h2>
		Simply pull this repo down and add the project into your projects solution.
		<br>
		Once included there are several calls you can make ,which are shown below.
		<h2>How do I get a every police force</h2>
		<pre>var AllPoliceForces = CrimeService.GetAllForces();</pre>

		<h2>How do I get a more info on a certain police force ie Wiltshire Police</h2>
		<pre>var PoliceForce = CrimeService.GetSingleForces("wiltshire");</pre>

		<h2>How do I get all crimes for a certain date in a certain location</h2>
		<pre>var Crimes = CrimeService.GetAllCrimesByPoint("52.9534161", "-1.1492773","2018-10");</pre>
	</div>
</div>

