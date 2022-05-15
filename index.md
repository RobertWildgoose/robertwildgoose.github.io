---
layout: default
title: "Portfolio"
---
  <div class="container-fluid">
    <div class="row title_header">
      <center>
        <h1>Work Experience</h1>
      </center>
    </div>
    <div class="row work_experience">
      <div class="col-4 col-md-4 col-sm-12">
        <center>
          <h3 class="work_title">Senior Mobile Apps Developer</h3>
          <h5>Next Technology</h5>
          <p class="mb-0 opacity-75">Jul 2021 - Present</p>
        </center>
      </div>
      <div class="col-4 col-md-4 col-sm-12"> 
        <center>
          <h3 class="work_title">Mobile Apps Developer</h3>
          <h5>Next Technology</h5>
          <p class="mb-0 opacity-75">Aug 2017 – Jul 2021</p>
        </center>
      </div>
      <div class="col-4 col-md-4 col-sm-12">
        <center>
          <h3 class="work_title">Trainee Mobile Apps Developer</h3>
          <h5>Next Technology</h5>
          <p class="mb-0 opacity-75">Jul 2016 – Aug 2017</p>
        </center>
      </div>
    </div>
    <div class="row title_header">
      <center>
        <hr>
        <h1>iOS Applications</h1>
      </center>
    </div>
    <div class="row work_experience">
      {% for post in site.posts %}
        {% if(post.type == "iOS") %}
        <div class="col-4 col-md-4 col-sm-12">
          <a href="{{site.baseurl}}{{ post.url }}" style="color: black;">
            <center>
              <img class="app_icon_image" src="{{ site.baseurl }}/{{post.image}}">
              <h3 class="work_title">{{post.title}}</h3>
              <h5>{{post.subtitle}}</h5>
              <h6>{{post.currentVersion}}</h6>
            </center>
          </a>
        </div>
        {% endif %}
      {% endfor %}
    </div>
    <div class="row title_header">
      <center>
        <hr>
        <h1>Mac Applications</h1>
      </center>
    </div>
     <div class="row work_experience">
      {% for post in site.posts %}
        {% if(post.type == "Mac") %}
        <div class="col-4 col-md-4 col-sm-12">
          <a href="{{site.baseurl}}{{ post.url }}" style="color: black;">
            <center>
              <img class="app_icon_image" src="{{ site.baseurl }}/{{post.image}}">
              <h3 class="work_title">{{post.title}}</h3>
              <h5>{{post.subtitle}}</h5>
            </center>
          </a>
        </div>
        {% endif %}
      {% endfor %}
    </div>
    <div class="row title_header">
      <center>
        <hr>
        <h1>Innovation Items</h1>
      </center>
    </div>
    <div class="row work_experience">
      {% for post in site.posts %}
        {% if(post.type == "POC") %}
        <div class="col-4 col-md-4 col-sm-12">
          <a href="{{site.baseurl}}{{ post.url }}" style="color: black;">
            <center>
              <img class="app_icon_image" src="{{ site.baseurl }}/{{post.image}}">
              <h3 class="work_title">{{post.title}}</h3>
              <h5>{{post.subtitle}}</h5>
            </center>
          </a>
        </div>
        {% endif %}
      {% endfor %}
    </div>
  </div>

