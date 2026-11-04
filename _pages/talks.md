---
layout: page
permalink: /talks/
title: talks
description: Conference, workshop and seminar presentations. Talks I gave more than once are listed once, with every occasion underneath.
nav: true
nav_order: 3
_styles: >
  .talk { margin-bottom: 2rem; }
  .talk h2 { font-size: 1.25rem; margin-bottom: 0.25rem; }
  .talk-meta { color: var(--global-text-color-light); margin-bottom: 0.5rem; }
  .talk-label { font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.05em; color: var(--global-theme-color); margin-left: 0.4rem; }
---

{%- comment -%} Edit the talks in _data/talks.yml, not here. {%- endcomment -%}
<div class="talk-list">
{%- for talk in site.data.talks -%}
{%- assign occasions = talk.given | sort: "date" | reverse -%}
<div class="talk">
<h2>{{ talk.title }}</h2>
<p class="talk-meta">
{%- if talk.coauthors -%}Joint work with {{ talk.coauthors }}{%- endif -%}
{%- if occasions.size > 1 -%}{%- if talk.coauthors %} · {% endif -%}Given {{ occasions.size }} times{%- endif -%}
{%- if talk.slides %} · <a href="{{ talk.slides | relative_url }}">slides</a>{%- endif -%}
</p>
<table class="table table-sm table-borderless">
{%- for g in occasions -%}
<tr><th scope="row" style="width: 20%">{{ g.date | date: "%b %Y" }}</th><td>{{ g.event }}{% if g.place %}, {{ g.place }}{% endif %}{% if g.invited %}<span class="talk-label">invited</span>{% endif %}</td></tr>
{%- endfor -%}
</table>
</div>
{%- endfor -%}
</div>
