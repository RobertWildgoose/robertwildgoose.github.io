---
layout: landingPage
title: "Happy Jekylling!"
---
<link
  rel="stylesheet"
  href="https://rawgit.com/kremalicious/appstorebadges/master/dist/appstorebadges.min.css"
/>
<div id="mobile_apps" class="background-alt">
    <center>
        <h2 class="heading">Release Notes</h2><hr>
        <a class="badge" href="#">
          <svg class="badge__icon">[…]</svg>
          <span class="badge__text">Download on the</span>
          <span class="badge__storename">App Store</span>
        </a>
    </center>
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