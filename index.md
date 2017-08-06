---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

<div id="container" class="shadow">
  <div class="content">
    <img class="big-logo" src="/assets/widyatama-studio-logo.png">
    <h1 class="title">Widyatama.Studio</h1>
    <h3 class="name">Ratnasari Widyatama Putri</h3>
    <div class="jobs monospace">architect</div>
  </div>
</div>

<div id="works">
  <h2 class="anchor">Works.</h2>
  {% assign iteration = 0 %}
  {% for post in site.posts %}
    <a href="{{ post.url }}">
      <div class="work shadow">
        <img class="work-cover" src="/images/{{ post.image-folder }}/{{ post.cover }}.jpg">
        <div class="work-content">
          <h3 class="work-title">{{ post.title }}</h3>
          <table class="monospace">
            <tr><td>Project type</td><td>{{ post.project_type }}</td></tr>
            <tr><td>Client</td><td>{{ post.client }}</td></tr>
            <tr><td>Location</td><td>{{ post.location }}</td></tr>
            <tr><td>Site area</td><td>{{ post.area }} m<sup>2</sup></td></tr>
            <tr><td>Building area</td><td>{{ post.building_area }} m<sup>2</sup></td></tr>
            <tr><td>Project year</td><td>{{ post.project_year }}</td></tr>
          </table>
        </div>
        <div class="clear"></div>
      </div>
    </a>
  {% endfor %}
</div>

<script src="https://soulwire.github.io/sketch.js/js/sketch.min.js"></script>
<script src="/assets/subdiv.js"></script>