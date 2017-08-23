---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

<div id="container" class="shadow wrapper">
  <div class="content">
    <img class="big-logo" src="/assets/widyatama-studio-logo.png">
    <h1 class="title">Widyatama.Studio</h1>
    <h3 class="name">Ratnasari Widyatama Putri</h3>
    <div class="jobs monospace">architect</div>
  </div>
</div>

<div id="works">
  <div class="wrapper">
    <h2 class="anchor">Recent Works.</h2>
    {% for post in site.posts limit:2 %}
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
  <div class="post-btn-list">
    <a href='/works'>
      <button class="btn red shadow monospace">View more.</button>
    </a>
  </div>
</div>

<div id="contact">
  <div class="wrapper">
    <h2 class="anchor">Get in touch.</h2>
    <table class="monospace">
      <tr>
        <td>Phone</td>
        <td>:</td>
        <td>+62 081 227 028 645</td>
      </tr>
      <tr>
        <td>Email</td>
        <td>:</td>
        <td><a href="mailto:contact@widyatama.studio">contact@widyatama.studio</a></td>
      </tr>
      <tr>
        <td>LINE</td>
        <td>:</td>
        <td>widyatamaputri</td>
      </tr>
      <tr>
        <td>LinkedIn</td>
        <td>:</td>
        <td>
        <a href="https://www.linkedin.com/in/widyatamaputri/">https://www.linkedin.com/in/widyatamaputri/</a></td>
      </tr>
      <tr>
        <td>Facebook</td>
        <td>:</td>
        <td><a href="https://www.facebook.com/widyatamap">https://www.facebook.com/widyatamap</a></td>
      </tr>
      <tr>
        <td>Framesia</td>
        <td>:</td>
        <td><a href="https://framesia.com/u/nana">https://framesia.com/u/nana</a></td>
      </tr>
    </table>

    <p class="small">
      Surakarta, Indonesia<br />© 2017
    </p>
  </div>
</div>


<script src="https://soulwire.github.io/sketch.js/js/sketch.min.js"></script>
<script src="/assets/subdiv.js"></script>