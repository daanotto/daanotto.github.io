---
layout: page
permalink: /teaching/
title: teaching
description: Courses I have taught or assisted, and students I have supervised.
nav: false # set to true once _data/teaching.yml has entries
nav_order: 4
---

{%- comment -%} Edit your teaching in _data/teaching.yml, not here. {%- endcomment -%}
<div class="teaching-list">
{%- assign t = site.data.teaching -%}
{%- if t.courses.size > 0 -%}
<h2>Courses</h2>
<table class="table table-sm table-borderless">
{%- for c in t.courses -%}
<tr><th scope="row" style="width: 20%">{{ c.years }}</th><td><strong>{{ c.course }}</strong><br>{{ c.role }}{% if c.programme %} · {{ c.programme }}{% endif %}{% if c.institution %}, {{ c.institution }}{% endif %}</td></tr>
{%- endfor -%}
</table>
{%- endif -%}
{%- if t.supervision.size > 0 -%}
<h2>Thesis supervision</h2>
<table class="table table-sm table-borderless">
{%- for s in t.supervision -%}
<tr><th scope="row" style="width: 20%">{{ s.years }}</th><td><strong>{{ s.student }}</strong>, {{ s.level }}<br><em>{{ s.title }}</em>{% if s.cosupervisor %} · co-supervised with {{ s.cosupervisor }}{% endif %}</td></tr>
{%- endfor -%}
</table>
{%- endif -%}
</div>
