---
layout: page
title: Research Area
permalink: /Research/
description: A growing collection of your cool projects.
nav: true
nav_order: 4
display_categories: [Research, Works]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="grid">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="grid">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>


<svg width="960" height="600" version="1.1" xmlns="http://www.w3.org/2000/svg"><g></g><g transform="translate(480,300)"><text text-anchor="middle" transform="translate(-34,-141)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(107, 110, 207);">Mobile</text><text text-anchor="middle" transform="translate(-9,118)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(156, 158, 222);">Cellular</text><text text-anchor="middle" transform="translate(-217,181)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(99, 121, 57);">Optimization</text><text text-anchor="middle" transform="translate(75,-168)rotate(-59.99999999999999)" style="font-size: 87px; font-family: Impact; fill: rgb(140, 162, 82);">MIMO</text><text text-anchor="middle" transform="translate(-327,40)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(181, 207, 107);">CommunicationsTheory</text><text text-anchor="middle" transform="translate(-102,123)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(206, 219, 156);">RIS</text><text text-anchor="middle" transform="translate(128,-189)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(140, 109, 49);">SignalProcessing</text><text text-anchor="middle" transform="translate(-258,-51)rotate(-59.99999999999999)" style="font-size: 48px; font-family: Impact; fill: rgb(189, 158, 57);">IAB</text><text text-anchor="middle" transform="translate(267,-81)rotate(-59.99999999999999)" style="font-size: 48px; font-family: Impact; fill: rgb(231, 186, 82);">SWIPT</text><text text-anchor="middle" transform="translate(29,-70)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(231, 203, 148);">mMIMO</text><text text-anchor="middle" transform="translate(253,-162)rotate(-59.99999999999999)" style="font-size: 48px; font-family: Impact; fill: rgb(132, 60, 57);">Wireless</text><text text-anchor="middle" transform="translate(177,104)rotate(-59.99999999999999)" style="font-size: 10px; font-family: Impact; fill: rgb(173, 73, 74);">5G</text><text text-anchor="middle" transform="translate(-75,122)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(214, 97, 107);">UAV</text><text text-anchor="middle" transform="translate(403,-42)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(231, 150, 156);">PhysicalLayer</text><text text-anchor="middle" transform="translate(-223,-49)rotate(59.99999999999999)" style="font-size: 87px; font-family: Impact; fill: rgb(123, 65, 115);">CellFree</text><text text-anchor="middle" transform="translate(159,72)rotate(0)" style="font-size: 10px; font-family: Impact; fill: rgb(165, 81, 148);">Security</text><text text-anchor="middle" transform="translate(-4,-74)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(206, 109, 189);">IRS</text><text text-anchor="middle" transform="translate(-44,8)rotate(59.99999999999999)" style="font-size: 100px; font-family: Impact; fill: rgb(222, 158, 214);">beamforming</text><text text-anchor="middle" transform="translate(-239,16)rotate(-59.99999999999999)" style="font-size: 48px; font-family: Impact; fill: rgb(57, 59, 121);">Deep</text><text text-anchor="middle" transform="translate(-110,108)rotate(0)" style="font-size: 48px; font-family: Impact; fill: rgb(82, 84, 163);">Learning</text><text text-anchor="middle" transform="translate(187,116)rotate(-59.99999999999999)" style="font-size: 10px; font-family: Impact; fill: rgb(107, 110, 207);">Integrated</text><text text-anchor="middle" transform="translate(300,-109)" style="font-size: 10px; font-family: Impact; fill: rgb(156, 158, 222);">Access</text><text text-anchor="middle" transform="translate(171,-163)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(99, 121, 57);">Backhaul</text><text text-anchor="middle" transform="translate(352,-69)rotate(-59.99999999999999)" style="font-size: 71px; font-family: Impact; fill: rgb(140, 162, 82);">Massive</text><text text-anchor="middle" transform="translate(-306,-161)rotate(-59.99999999999999)" style="font-size: 71px; font-family: Impact; fill: rgb(181, 207, 107);">systems</text><text text-anchor="middle" transform="translate(-322,77)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(206, 219, 156);">SystemsEnergy</text><text text-anchor="middle" transform="translate(-232,36)rotate(-59.99999999999999)" style="font-size: 10px; font-family: Impact; fill: rgb(140, 109, 49);">Efficient</text><text text-anchor="middle" transform="translate(173,-126)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(189, 158, 57);">AP</text><text text-anchor="middle" transform="translate(332,44)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(231, 203, 148);">Reinforcement</text><text text-anchor="middle" transform="translate(-159,-125)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(132, 60, 57);">Approach</text><text text-anchor="middle" transform="translate(-58,-165)rotate(59.99999999999999)" style="font-size: 10px; font-family: Impact; fill: rgb(173, 73, 74);">Power</text><text text-anchor="middle" transform="translate(-287,-99)rotate(0)" style="font-size: 10px; font-family: Impact; fill: rgb(214, 97, 107);">Allocation</text><text text-anchor="middle" transform="translate(-211,102)rotate(-59.99999999999999)" style="font-size: 10px; font-family: Impact; fill: rgb(231, 150, 156);">Downlink</text><text text-anchor="middle" transform="translate(-334,-37)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(123, 65, 115);">Training</text><text text-anchor="middle" transform="translate(163,17)rotate(59.99999999999999)" style="font-size: 100px; font-family: Impact; fill: rgb(165, 81, 148);">Networks</text><text text-anchor="middle" transform="translate(84,-31)rotate(59.99999999999999)" style="font-size: 48px; font-family: Impact; fill: rgb(222, 158, 214);">multiIRS</text><text text-anchor="middle" transform="translate(-237,118)rotate(-59.99999999999999)" style="font-size: 48px; font-family: Impact; fill: rgb(82, 84, 163);">Reflecting</text><text text-anchor="middle" transform="translate(-318,162)rotate(-59.99999999999999)" style="font-size: 48px; font-family: Impact; fill: rgb(156, 158, 222);">Cognitive</text><text text-anchor="middle" transform="translate(-330,26)rotate(-29.999999999999993)" style="font-size: 48px; font-family: Impact; fill: rgb(99, 121, 57);">Radio</text><text text-anchor="middle" transform="translate(-354,104)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(140, 162, 82);">Secure</text><text text-anchor="middle" transform="translate(21,170)rotate(-59.99999999999999)" style="font-size: 10px; font-family: Impact; fill: rgb(181, 207, 107);">Millimeter</text><text text-anchor="middle" transform="translate(141,51)" style="font-size: 10px; font-family: Impact; fill: rgb(206, 219, 156);">Wave</text><text text-anchor="middle" transform="translate(199,131)" style="font-size: 10px; font-family: Impact; fill: rgb(140, 109, 49);">3D</text><text text-anchor="middle" transform="translate(165,153)rotate(59.99999999999999)" style="font-size: 10px; font-family: Impact; fill: rgb(189, 158, 57);">Surface</text><text text-anchor="middle" transform="translate(210,151)rotate(0)" style="font-size: 10px; font-family: Impact; fill: rgb(231, 186, 82);">Vertical</text><text text-anchor="middle" transform="translate(-46,-179)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(231, 203, 148);">SurfaceAided</text><text text-anchor="middle" transform="translate(302,106)rotate(59.99999999999999)" style="font-size: 10px; font-family: Impact; fill: rgb(132, 60, 57);">ANaided</text><text text-anchor="middle" transform="translate(-151,-149)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(173, 73, 74);">Secrecy</text><text text-anchor="middle" transform="translate(0,63)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(214, 97, 107);">rate</text><text text-anchor="middle" transform="translate(-190,-187)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(231, 150, 156);">maximization</text><text text-anchor="middle" transform="translate(-194,-159)rotate(0)" style="font-size: 10px; font-family: Impact; fill: rgb(123, 65, 115);">mmWave</text><text text-anchor="middle" transform="translate(87,-145)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(82, 84, 163);"></text><text text-anchor="middle" transform="translate(-104,-8)rotate(59.99999999999999)" style="font-size: 48px; font-family: Impact; fill: rgb(206, 109, 189);">multiuser</text><text text-anchor="middle" transform="translate(75,41)rotate(59.99999999999999)" style="font-size: 48px; font-family: Impact; fill: rgb(57, 59, 121);">Intelligent</text><text text-anchor="middle" transform="translate(-108,163)rotate(0)" style="font-size: 48px; font-family: Impact; fill: rgb(107, 110, 207);">IRSassisted</text><text text-anchor="middle" transform="translate(-21,-202)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(165, 81, 148);">Optimum</text><text text-anchor="middle" transform="translate(271,42)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(231, 150, 156);">Solutions</text><text text-anchor="middle" transform="translate(220,176)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(189, 158, 57);">Weighted</text><text text-anchor="middle" transform="translate(-139,-37)rotate(59.99999999999999)" style="font-size: 10px; font-family: Impact; fill: rgb(181, 207, 107);">SumRate</text><text text-anchor="middle" transform="translate(158,86)rotate(0)" style="font-size: 10px; font-family: Impact; fill: rgb(222, 158, 214);">NOMA</text><text text-anchor="middle" transform="translate(-42,-212)rotate(-59.99999999999999)" style="font-size: 10px; font-family: Impact; fill: rgb(206, 109, 189);">TDMA</text><text text-anchor="middle" transform="translate(321,69)rotate(-29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(231, 186, 82);">Powered</text><text text-anchor="middle" transform="translate(-20,-91)rotate(29.999999999999993)" style="font-size: 10px; font-family: Impact; fill: rgb(57, 59, 121);">IoT</text></g></svg>