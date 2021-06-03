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

<!-- <div id="mobile_apps" class="background-alt">
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
</div> -->
<div id="iOS_apps" class="background-alt">
    <center><h2 class="heading">iOS Apps</h2></center>
    <div class="container pt">
        <div class="row mt centered">   
            <div class="col-lg-4">
                <a class="zoom green" href="morsed.html"><img class="img-responsive" src="assets/images/morsed.jpg" alt="" />
                <p>Morsed - V2.1.0</p></a>
            </div>
            <div class="col-lg-4">
                <a class="zoom green" href="todaily.html"><img class="img-responsive" src="assets/images/todaily.jpg" alt="" />
                <p>Todaily - V2.6.0</p></a>
            </div>
            <div class="col-lg-4">
                <a class="zoom green" href="spellthatforme.html"><img class="img-responsive" src="assets/images/spellthatforme.jpg" alt="" />
                <p>Spell That For Me - V1.0.2</p></a>
            </div>
        </div>
    </div>
</div>
<div id="mac_apps" class="background-alt">
    <center><h2 class="heading">Mac Apps</h2></center>
    <div class="container pt">
        <div class="row mt centered">   
            <div class="col-lg-4">
                <a class="zoom green" href="https://robertwildgoose.github.io/assets/AppIconGenerator.zip"><img class="img-responsive" src="assets/images/appicongenerator.jpg" alt="" />
                <p>App Icon Generator V1.0</p></a>
            </div>
            <div class="col-lg-4">
                <a class="zoom green"><img class="img-responsive" src="assets/images/grey-square.png" alt="" />
                <p></p></a>
            </div>
            <div class="col-lg-4">
                <a class="zoom green"><img class="img-responsive" src="assets/images/grey-square.png" alt="" />
                <p></p></a>
            </div>
        </div>
    </div>
</div>
<!-- <div id="code_libraries" class="background-alt">
    <center><h2 class="heading">Libraries</h2></center>
    <div class="container pt">
        <div class="row mt centered">   
            <div class="col-lg-4">
                <a class="zoom green" href="morsed.html"><img class="img-responsive" src="assets/img/portfolio/port01.jpg" alt="" />
                <p>Morsed - V2.1.0</p></a>
            </div>
            <div class="col-lg-4">
                <a class="zoom green" href="work01.html"><img class="img-responsive" src="assets/img/portfolio/port02.jpg" alt="" />
                <p>Todaily - V2.6.0</p></a>
            </div>
            <div class="col-lg-4">
                <a class="zoom green" href="work01.html"><img class="img-responsive" src="assets/img/portfolio/port03.jpg" alt="" />
                <p>Spell That For Me - V1.0.2</p></a>
            </div>
        </div>
        <div class="row mt centered">   
            <div class="col-lg-4">
                <a class="zoom green" href="work01.html"><img class="img-responsive" src="assets/img/portfolio/port04.jpg" alt="" />
                <p>App Icon Generator V1.0</p></a>
            </div>
        </div>
    </div>
</div> -->
<div id="education">
    <h2 class="heading">Education</h2>
    {% for post in site.education %}
		<div class="education-block">
			<center><img style="width:50px;" src="{{post.imageUrl}}"></center>
			<center>{{post.title}}<br>{{post.completedate}}</center>
    	</div>
    {% endfor %}
</div>