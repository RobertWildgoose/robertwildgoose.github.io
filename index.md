---
layout: default
title: "Portfolio"
---
<div class="row title_header">
  <center>
    <img style="width: 80%;" src="{{ site.baseurl }}/assets/headerbar.png"/>
  </center>
</div>
<div class="row title_header">
    <center>
      <h1>Experience</h1>
    </center>
  </div>
  <div class="row">
    <div class="col-12 col-md-12 col-sm-12">
      <div class="row row-cols-1 row-cols-md-3 mb-3 text-center">
      <div class="col-4 col-md-6 col-sm-12">
        <div class="card mb-4 rounded-3 shadow-sm border-primary">
          <div class="card-header py-3 text-white bg-primary border-primary">
            <h4 class="my-0 fw-normal">Mobile Apps Developer</h4>
          </div>
          <div class="card-body">
            <img src="https://wl3-cdn.landsec.com/sites/default/files/images/shops/logos/pure-gym_0.png" style="width: 150px;height: 150px;"/>
            <h3 class="card-title pricing-card-title">Pure Gym</h3>
            <h4><small class="text-muted fw-light">Aug 2022 - Present</small></h4>
          </div>
        </div>
      </div>
      <div class="col-4 col-md-6 col-sm-12">
        <div class="card mb-4 rounded-3 shadow-sm">
          <div class="card-header py-3 text-black">
            <h4 class="my-0 fw-normal">Senior Mobile Apps Developer</h4>
          </div>
          <div class="card-body">
            <img src="https://www.nextplc.co.uk/~/media/Images/N/Next-PLC-V2/content-images/image-gallery/logos/next-white-v2-logo.jpg?w=767" style="width: 150px;height: 150px;"/>
            <h3 class="card-title pricing-card-title">Next Technology</h3>
            <h4><small class="text-muted fw-light">Jul 2021 - Aug 2022</small></h4>
          </div>
        </div>
      </div>
      <div class="col-4 col-md-6 col-sm-12">
        <div class="card mb-4 rounded-3 shadow-sm">
          <div class="card-header py-3 text-black">
            <h4 class="my-0 fw-normal">Mobile Apps Developer</h4>
          </div>
          <div class="card-body">
            <img src="https://www.nextplc.co.uk/~/media/Images/N/Next-PLC-V2/content-images/image-gallery/logos/next-white-v2-logo.jpg?w=767" style="width: 150px;height: 150px;"/>
            <h3 class="card-title pricing-card-title">Next Technology</h3>
            <h4><small class="text-muted fw-light">Aug 2017 – Jul 2021</small></h4>
          </div>
        </div>
      </div>
      <div class="col-4 col-md-6 col-sm-12">
        <div class="card mb-4 rounded-3 shadow-sm">
          <div class="card-header py-3 text-black">
            <h4 class="my-0 fw-normal">Trainee Mobile Apps Developer</h4>
          </div>
          <div class="card-body">
            <img src="https://www.nextplc.co.uk/~/media/Images/N/Next-PLC-V2/content-images/image-gallery/logos/next-white-v2-logo.jpg?w=767" style="width: 150px;height: 150px;"/>
            <h3 class="card-title pricing-card-title">Next Technology</h3>
            <h4><small class="text-muted fw-light">Jul 2017 – Aug 2018</small></h4>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="row title_header">
    <center>
      <h1>Portfolio</h1>
    </center>
  </div>
  <div class="row work_experience">
    {% for post in site.posts %}
      {% if(post.type == "Application") %}
      <div class="col-4 col-md-4 col-sm-12" style="padding: 20px;">
        <img src="{{ site.baseurl }}/{{post.image}}" style="width:100%; border-radius: 15px; border: 2px grey solid;">
        <center>
          <h3 class="mb-0">{{post.title}}</h3>
          <div class="mb-1 text-muted">{{post.currentVersion}}</div>
          <p class="card-text mb-auto">{{post.subtitle}}</p>
          <a href="{{site.baseurl}}{{ post.url }}"><button type="button" class="btn btn-primary btn-lg px-4 gap-3 link-button">More Info</button></a>
          {% if post.link != "" %}
                 <a href="{{ post.link }}"><button type="button" class="link-button btn btn-primary btn-lg px-4 gap-3">View App</button></a>
              {% endif %}
        </center>
      </div>
      {% endif %}
    {% endfor %}
  </div>
</div>

