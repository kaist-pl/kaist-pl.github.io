---
layout: default
title: Home
---

<!-- Background image -->
<div id="carouselExampleSlidesOnly" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <div class="p-5 text-center bg-image" style="
        background-image: url('images/CampusBgDay.png');
        background-size:cover;
        height: 400px;
      ">
        <div class="mask" style="background-color: rgba(0, 0, 0, 0.6);">
          <div class="d-flex justify-content-center align-items-center h-100">
            <div class="text-white">
              <h1 class="mb-3">Programming Langauges @ KAIST</h1>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="carousel-item">
      <div class="p-5 text-center bg-image" style="
        background-image: url('images/CampusBgNight.png');
        background-size:cover;
        height: 400px;
      ">
        <div class="mask" style="background-color: rgba(0, 0, 0, 0.6);">
          <div class="d-flex justify-content-center align-items-center h-100">
            <div class="text-white">
              <h1 class="mb-3">Programming Langauges @ KAIST</h1>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="carousel-item">
      <div class="p-5 text-center bg-image" style="
        background-image: url('images/kaist.jpg');
        background-size:cover;
        height: 400px;
      ">
        <div class="mask" style="background-color: rgba(0, 0, 0, 0.6);">
          <div class="d-flex justify-content-center align-items-center h-100">
            <div class="text-white">
              <h1 class="mb-3">Programming Langauges @ KAIST</h1>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
<!-- Background image -->

<br>
# Introduction
<p class="lead">
We are a group of researchers in programming languages at KAIST.
Our goal is to understand the principles of programming languages for developing reliable
and efficient software systems. Our research topics include type theories, formal verification,
program analysis, program synthesis, concurrency, parallelism, probabilistic programming, and computational learning
theories. For detailed information, please visit the websites of each faculty member
and research lab listed below.
</p>

---

# Faculty
<div class="staff-profiles">
{% for faculty in site.data.faculty %}

<div class="profile">
<img alt="{{ faculty.name }}" src="images/{{ faculty.short }}.jpg"/>

<p>
  <br/>
  <h5 style="display: inline">{{ faculty.name }}</h5>
  <a class="staff-name" href="{{ faculty.website }}"><i class="icon fa fa-home"></i></a>
  <a href="mailto:{{ faculty.email }}"><i class="icon fa fa-envelope"></i></a>
  <br/>
  <h6 style="display: inline">{{ faculty.lab }}</h6>
  <a class="staff-name" href="{{ faculty.lab-website }}"><i class="icon fa fa-home"></i></a>
  <a href="mailto:{{ faculty.lab-mailing-list }}"><i class="icon fa fa-envelope"></i></a>
</p>
</div>
{% endfor %}
</div>
<br>

---

# Course
{% for course in site.data.course %}
- <h5><a href="{{ course.website }}">{{ course.name }}</a></h5>
{% endfor %}
