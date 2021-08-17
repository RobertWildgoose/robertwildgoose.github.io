---
layout: default
title: "Happy Jekylling!"
---

<div style="margin:20px;" id="socials">
    <center><h2 class="heading">Socials</h2></center>
    <div class="social-btns" style="padding:10px;">
    	<center>
		    <a href="{{site.github}}" target="_blank"><i class="fa fa-github" aria-hidden="true"></i></a>
		    <a href="{{site.linkedIn}}" target="_blank"><i class="fa fa-linkedin" aria-hidden="true"></i></a>
		    <a href="{{site.apple}}" target="_blank"><i class="fa fa-apple" aria-hidden="true"></i></a>
		    <a href="{{site.twitter}}" target="_blank"><i class="fa fa-twitter" aria-hidden="true"></i></a>
		</center>
	</div>
</div>

<div id="skills">
    <h2 class="heading">Skills</h2>
    <ul>
    	<li>Swift</li>
        <li>Mac Development</li>
        <li>iOS Development</li>
        <li>C#</li>
        <li>Xamarin</li>
    </ul>
</div>

<div id="mobile_apps" class="background-alt">
    <center><h2 class="heading">iOS Apps</h2></center>
    <div class="container">
        <div class="row">
    	  {% for post in site.mobile_apps %}
		  <div class="project shadow-large">
		  	<div class="project-image">
		  		<img src="{{post.image}}" />
		  	</div>
		  	<div class="project-info">
		  		<h2>{{post.title}}</h2>
		  		<p>{{post.content}}</p>
		  		<a href="{{post.link}}" {{post.downloadable}}>View Project</a>
		  	</div>
		  </div>
		  {% endfor %}
        </div>
    </div>
</div>
<div class="container pt">
    <div class="row mt centered">
        {% for post in site.posts %}
            <div class="col-lg-4">
                <a class="zoom green" href="{{post.link}}"><img class="img-responsive" src="assets/{{post.image}}" alt="" />
                <p>{{post.title}}</p></a>
            </div>
        {% endfor %}
    </div>
</div>
<div id="education">
    <h2 class="heading">Education</h2>
    {% for post in site.education %}
		<div class="education-block">
			<center><img style="width:50px;" src="{{post.imageUrl}}"></center>
			<center>{{post.title}}<br>{{post.completedate}}</center>
    	</div>
    {% endfor %}
</div>