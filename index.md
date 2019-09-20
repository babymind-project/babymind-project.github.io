---
layout: default
title: Babymind
---

<link rel="stylesheet" href="/assets/css/member.css">
<link rel="stylesheet" href="/assets/css/index.css">
<script type="text/javascript" src="/assets/js/index.js"></script>

<div class="bk-container">
  <img class="bk-img" src="/assets/images/main.png">
  <h2 class="bk-header">
    <i> Building Infant-Mimic Neurocognitive AI </i>
  </h2>
</div>

<!--<div class="update content-container">
  <h1 class = "content-title">
    Updates
  </h1>
  {% for news in site.data.updates %}
  <p class="content-item news news-{{ forloop.index0 }}">
    <span id="date">{{ news.date }}</span>
    {{ news.content }}
  </p>
  {% endfor %}
  <p class="content-item showMore">
    <span id="more" onclick="showMore()">More</span>
<span id="noMoreContext" style="display:none;color: #cccccc;"><br>No more news available.</span>
  </p>
</div>-->

<div class="about content-container">
  <h2 class = "content-title">
    What is Babymind Project?
  </h2>
  <p class="content-item">
   Babymind is a research project which aims to build infant-mimic neuro-cognitive AI technologies. Our project consists of four sub-teams that are responsible for knowledge integration, vision-audio, language-emotion, and robot-behavior. We are planning to experiment our project in real and virtual-reality-based environments.     
  </p>
</div>

<div class="people content-container">
  <h2 class = "content-title">
    People
  </h2>
  <div class="content-item">
    {% for person in site.data.people %}
      <div class="member">
        <div class="member-profile">
          <img class="member-profile" src="{{person.src}}">
        </div>
        <div class="member-info member-name">
          {{ person.name }}
        </div>
        <div class="member-info member-position">
          {{ person.affiliation }}
        </div>
      </div>
    {% endfor %}
  </div>
</div>
