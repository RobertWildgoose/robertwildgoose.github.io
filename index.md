---
layout: default
title: "Happy Jekylling!"
---

<div style="margin:5px;">
    <center><h2 class="heading" style="margin:30px;">Socials</h2></center>
    <div class="social-btns" style="padding:5px;">
    	<center>
		    <a href="{{site.github}}" target="_blank"><i class="fa fa-github" aria-hidden="true"></i></a>
		    <a href="{{site.linkedIn}}" target="_blank"><i class="fa fa-linkedin" aria-hidden="true"></i></a>
		    <a href="{{site.apple}}" target="_blank"><i class="fa fa-apple" aria-hidden="true"></i></a>
		    <a href="{{site.twitter}}" target="_blank"><i class="fa fa-twitter" aria-hidden="true"></i></a>
		</center>
	</div>
</div>

<div id="skills" class="background-alt">
    <h2 class="heading" style="margin:30px;">Skills</h2>
    <ul>
    	<li>Swift</li>
        <li>Mac Development</li>
        <li>iOS Development</li>
        <li>C#</li>
        <li>Xamarin</li>
    </ul>
</div>

<div id="mobile_apps" style="margin:20px;">
    <div class="container-fluid">
        <div class="row">
            <div class="col-12 col-sm-12 col-md-12">
                <center><h2 class="heading" style="margin:30px;">Experience</h2></center>
            </div>
        </div>
        <div class="row">
            <div class="col-12 col-sm-12 col-md-12">
                <center>
                    <h3 class="heading" style="margin:30px;">NEXT PLC</h3>
                </center>
            </div>
        </div>
        <div class="row">
            <div class="col-12 col-sm-4 col-md-4">
                <center>
                    <div class="card" style="width: 80%;">
                        <div class="card-body">
                        <h3 class="card-title">Senior Mobile Apps Developer</h3>
                        <h6 class="card-subtitle mb-2 text-muted">2021 - Present</h6>
                      </div>
                    </div>
                </center>
            </div>
            <div class="col-12 col-sm-4 col-md-4">
                <center>
                    <div class="card" style="width: 80%;">
                        <div class="card-body">
                        <h3 class="card-title">Mobile Apps Developer</h3>
                        <h6 class="card-subtitle mb-2 text-muted">2017 - 2021</h6>
                      </div>
                    </div>
                </center>
            </div>
            <div class="col-12 col-sm-4 col-md-4">
                <center> 
                <div class="card" style="width: 80%;">
                    <div class="card-body">
                    <h3 class="card-title">Trainee Mobile Apps Developer</h3>
                    <h6 class="card-subtitle mb-2 text-muted">2016 - 2017</h6>
                  </div>
                </div>      
                </center>
            </div>
        </div>
    </div>
</div>
<div id="mobile_apps" class="background-alt">
    <center>
        <h2 class="heading" style="margin:30px;">Projects</h2>
    </center>
    <div class="container-fluid">
        <div class="container pt">
            <div class="row mt centered">
                {% for post in site.posts %}
                    <div class="col-lg-4">
                        <a class="zoom green" href="{{ post.url }}"><img class="img-responsive" src="{{ site.baseurl }}/{{post.image}}" alt="" />
                        <center><p>{{post.title}}</p></center>
                        </a>
                    </div>
                {% endfor %}
            </div>
        </div>
    </div>
</div>