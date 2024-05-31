---
layout: page
permalink: /program/
title: Program
description: (Tentative)
nav: true
nav_order: 6
---
<hr>
<h3>Workshop program</h3>
<ul> 
    <li>Introduction of the drafted journal structure that will serve as pivotal discussion guideline during the workshop</li>
    <li>Invited speakers' presentations followed by interactive activities to engage the audience and collect different perspectives on the topics</li>
    <li>Breakout sessions to discuss the topics in smaller groups</li>
    <li>Plenary session to present the results of the breakout sessions</li>
    <li>Panel session</li>
    <li>Closing remarks and definition of plan of action for the scientific contribution</li>
</ul>


<h3>The Keynote Speaker: </h3>
<div class="row" style="display: flex; justify-content: center;">
  <div class="col-md-3 pr-0 pl-0 m-1" style = "min-height: 400px; max-width: 255px;">
      <div class="card p-1" style="min-height: inherit;">
        <a href="https://laurelriek.org/" target="_blank">
            <img src="/assets/img/lr.jpg" class="card-img-top speaker-img" alt="Lauriel Riek">
        </a>
        <div class="card-body p-2">
            <h5 class="card-title">Lauriel Riek</h5>
            <p class="card-text">Professor of Computer Science and Engineering</p>
            <p class="card-text">UC San Diego</p>
        </div>
        <div class="card-footer text-muted small p-2">
            In person <i class='fa-solid fa-user'></i>
        </div>
      </div>
  </div>
  <div class="col-md-6 m-1 pr-0 pl-0 d-inline">
      <div class="card p-1" style="min-height: inherit;">
      <div class="card-header"><h3>Title</h3></div>
      <div class="card-body">Abstract: TBD</div>
      </div>
  </div>
</div>
<hr>

<h3>Panel session #1: </h3>
   <div id="myCarouselSpeakers" class="carousel container card-deck mt-3 mb-5">
      <div class="carousel-inner w-100">  
        {% assign speakers = site.data.speakers.speakers | where: "session", "Session1" %}
        {% for speaker in speakers %}
            <div class="carousel-item {% if forloop.first %}active{% endif %}">
              <div class="col-md-3 my-1 pr-0 pl-0 h-100">
                <div class="card p-1">
                <a href="{{ speaker.website }}" target="_blank">
                  <img src="{{ speaker.image }}" class="card-img-top speaker-img" alt="{{ speaker.name }}">
                </a>
                <div class="card-body p-2">
                  <h5 class="card-title">{{ speaker.name }}</h5>
                  <p class="card-text">{{ speaker.title }}</p>
                  <p class="card-text">{{ speaker.affiliation }}</p>
                </div>
                  <div class="card-footer text-muted small p-2">
                      {{ speaker.attendance }}
                  </div>
              </div>
            </div>
          </div>
        {% endfor %}
      </div>
    </div>

<h3>Panel session #2: </h3>
<div id="myCarouselSpeakers" class="carousel container card-deck mt-3 mb-5">
      <div class="carousel-inner w-100">  
        {% assign speakers = site.data.speakers.speakers | where: "session", "Session2" %}
        {% for speaker in speakers %}
            <div class="carousel-item {% if forloop.first %}active{% endif %}">
              <div class="col-md-3 my-1 pr-0 pl-0 h-100">
                <div class="card p-1">
                <a href="{{ speaker.website }}" target="_blank">
                  <img src="{{ speaker.image }}" class="card-img-top speaker-img" alt="{{ speaker.name }}">
                </a>
                <div class="card-body p-2">
                  <h5 class="card-title">{{ speaker.name }}</h5>
                  <p class="card-text">{{ speaker.title }}</p>
                  <p class="card-text">{{ speaker.affiliation }}</p>
                </div>
                  <div class="card-footer text-muted small p-2">
                      {{ speaker.attendance }}
                  </div>
              </div>
            </div>
          </div>
        {% endfor %}
      </div>
    </div>
