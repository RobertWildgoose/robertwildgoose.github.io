---
title:  "Random User Generator"
subtitle: "A C# Library"
layout: post
author: "Robert Wildgoose"
type: DevelopmentLibrary
avatar: "img/authors/robertwildgoose.png"
class: "devicon-csharp-plain colored"
image: "img/projects/RandomUserGeneratorCSharp.jpg"
date:   2015-01-01 12:12:12
link: https://github.com/RobertWildgoose/RandomUserLib
---



<div class="post-heading">
	<div class="post-image-container">
		<img class="project-logo" src="{{ site.baseurl }}/img/projects/RandomUserGenerator.jpg"/>
	</div>
	<div class="post-bio-container">
		<h2>What Is It and How Can I Use It</h2>
		C# Random User Library provides random user data for each call sent out.<br>
		Pulling down the code from github and add this to your project.
		<h2>How do I get a single user?</h2>
		<pre>var SingleUser = UserGeneratorService.GetSingleUser().results.ElementAtOrDefault(0);</pre>

		<h2>How do I get a certain amount of users?</h2>
		<pre>var MultipleUsers = UserGeneratorService.GetMultipleUsers(10).results;</pre>

		<h2>How do I get a previous user back again?</h2>
		<pre>var MultipleUsers = UserGeneratorService.GetSpecificUser(User.seed).results;</pre>

		<h2>How do I get a User from a specific Demographic?</h2>
		<pre>var SpanishUser = UserGeneratorService.GetSingleUserSpecificNationality(Nationality.Spain).results.ElementAtOrDefault(0);</pre>

		<h2>How do I get a Set Of 10 Users from a specific Demographic?</h2>
		<pre>var MultipleSpanishUser = UserGeneratorService.GetMultiUsersSpecificNationality(Nationality.Spain,10).results;</pre>

	</div>
</div>
