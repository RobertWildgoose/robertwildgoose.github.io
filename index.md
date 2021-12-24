---
layout: default
title: "Portfolio"
---
<div class="album py-5 bg-light">
        <div class="row"><center><h1 style="margin:10px;">Experiance</h1></center></div>
        <div class="container">
            <div class="list-group">
                <a class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
                <div class="d-flex gap-2 w-100 justify-content-between">
                      <div>
                        <h3 class="mb-0">Senior Mobile Apps Developer</h3>
                        <p class="mb-0 opacity-75">Next Technology.</p>
                      </div>
                      <small class="opacity-50 text-nowrap">Jul 2021 - Present</small>
                    </div>
                  </a>
                  <a class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
                    <div class="d-flex gap-2 w-100 justify-content-between">
                      <div>
                        <h3 class="mb-0">Mobile Apps Developer</h3>
                        <p class="mb-0 opacity-75">Next Technology.</p>
                      </div>
                      <small class="opacity-50 text-nowrap">Aug 2017 – Jul 2021</small>
                    </div>
                  </a>
                  <a class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
                    <div class="d-flex gap-2 w-100 justify-content-between">
                      <div>
                        <h3 class="mb-0">Trainee Mobile Apps Developer</h3>
                        <p class="mb-0 opacity-75">Next Technology.</p>
                      </div>
                      <small class="opacity-50 text-nowrap">Jul 2016 – Aug 2017</small>
                    </div>
                  </a>
                </div>
        </div>
        <div class="container">
            <div class="row"><center><h1 style="margin:30px;">iOS Apps</h1></center></div>
            <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
            {% for post in site.posts %}
                {% if(post.type == "iOS") %}
                <div class="col">
                  <div class="card shadow-sm">
                    <a href="{{site.baseurl}}{{ post.url }}" style="color: black;">
                      <img src="{{ site.baseurl }}/{{post.image}}" class="bd-placeholder-img card-img-top" width="100%"/>
                    </a>
                    <div class="card-body">
                      <p class="card-text"><h4>{{post.title}}</h4> <p class="lead text-muted" style="min-height:75px;">{{post.subtitle}}</p></p>
                      <div class="d-flex justify-content-between align-items-center">
                      </div>
                    </div>
                  </div>
                </div>
                {% endif %}
            {% endfor %}
            </div>
        </div>
        <div class="container">
            <div class="row"><center><h1 style="margin:30px;">Proof Of Concepts</h1></center></div>
            <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
            {% for post in site.posts %}
                {% if(post.type == "POC") %}
                <div class="col">
                  <div class="card shadow-sm">
                    <a href="{{site.baseurl}}{{ post.url }}" style="color: black;">
                      <img src="{{ site.baseurl }}/{{post.image}}" class="bd-placeholder-img card-img-top" width="100%"/>
                    </a>
                    <div class="card-body">
                      <p class="card-text"><h4>{{post.title}}</h4> <p class="lead text-muted" style="min-height:75px;">{{post.subtitle}}</p></p>
                      <div class="d-flex justify-content-between align-items-center">
                      </div>
                    </div>
                  </div>
                </div>
                {% endif %}
            {% endfor %}
            </div>
        </div>

