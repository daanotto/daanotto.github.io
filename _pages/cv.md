---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* PhD in Applied Mathematics, GitHub University, 2028 (expected)
* MSc in Business Analytics, VU Amsterdam, 2023
* MSc in Econometrics & Operations Research, VU Amsterdam, 2022
* BSc in Mathematics, Leiden University, 2020
* BSc in Physics, Leiden University, 2020

Work experience
======
* 05/2024-now: PhD Candidate
  * University of Amsterdam, Amsterdam Business School
  * Supervisor: Jannis Kurtz, Ilker Birbil

* 04/2023-04/2024: Data Scientist/Strategy Consultant
  * REWIRE (formerly known as MIcompany)
  * Various projects on data science and data strategy

* 09/2022-02/2023: Green Supply Chain Analyst
  * KLM, Royal Dutch Airlines
  * Defining CO2 metrics for the supply chain
  * Modelling the optimal global supply strategy involving emissions

* 2017-2022: Teaching Assistant
  * Leiden University, VU Amsterdam
  * Hosting tutorials of various mathematical courses for Bachelor's and Master's students

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
