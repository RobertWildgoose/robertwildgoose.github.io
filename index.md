---
layout: default
title: "Happy Jekylling!"
---
<div id="iphone_apps" class="background-alt">
    <center>
        <h2 class="heading" style="margin:30px;">iOS Apps</h2>
    </center>
    <div class="container-fluid">
        <div class="row">
            {% for post in site.posts %}
                {% if(post.type == "iOS") %}
                    <div class="col-6 col-xs-6 col-sm-4 col-md-3 projectparent">
                        <a href="{{site.baseurl}}{{ post.url }}">
                            <img class="app_icon image1" src="{{ site.baseurl }}/{{post.image}}" alt="post.title" />
                            <img style="width:70px;" class="image2" src="{{ site.baseurl }}/{{post.icon}}" alt="post.title" />
                        </a>
                    </div>
                {% endif %}
            {% endfor %}
        </div>
    </div>
</div>
<div id="mac_apps" class="background-alt">
    <center>
        <h2 class="heading" style="margin:30px;">Mac Apps</h2>
    </center>
    <div class="container-fluid">
        <div class="row">
            {% for post in site.posts %}
                {% if(post.type == "mac") %}
                    <div class="col-6 col-xs-6 col-sm-4 col-md-3 projectparent">
                        <a href="{{site.baseurl}}{{ post.url }}">
                            <img class="app_icon image1" src="{{ site.baseurl }}/{{post.image}}" alt="post.title" />
                            <img style="width:70px;" class="image2" src="{{ site.baseurl }}/{{post.icon}}" alt="post.title" />
                        </a>
                    </div>
                {% endif %}
            {% endfor %}
        </div>
    </div>
</div>
<div id="mac_apps" class="background-alt">
    <center>
        <h2 class="heading" style="margin:30px;">Innovation Concepts</h2>
    </center>
    <div class="container-fluid">
        <div class="row">
            {% for post in site.posts %}
                {% if(post.type == "POC") %}
                    <div class="col-6 col-xs-6 col-sm-4 col-md-3 projectparent">
                        <a href="{{site.baseurl}}{{ post.url }}">
                            <img class="app_icon image1" src="{{ site.baseurl }}/{{post.image}}" alt="post.title" />
                            <img style="width:70px;" class="image2" src="{{ site.baseurl }}/{{post.icon}}" alt="post.title" />
                        </a>
                    </div>
                {% endif %}
            {% endfor %}
        </div>
    </div>
</div>

