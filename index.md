---
title: Welcome
navbar: Home
---

Welcome to <strong class="has-text-usf-green">CS {{ site.data.info.code }} {{ site.data.info.name }}</strong> for <strong class="has-text-usf-green">{{ site.data.info.term }}</strong>. {{ site.data.info.blurb }}

## Upcoming Schedule

Here is the upcoming course schedule, which includes links to lecture material, assigned quizzes and homework, and more:

<style>
ul.icons {
  list-style-type: none;
  margin-left: 1.5em;
  margin-top: 0em;
}

ul.icons > li {
  position: relative;
}

ul.icons > li > i {
  width: 1.25em;
  left: -1.5em;
  position: absolute;
  text-align: center;
  line-height: inherit;
}

.content li.bump {
  margin-top: 0.8rem;
}
</style>
{% comment %}
{%- assign today_date = 'now' | date: '%Y-%m-%d' -%}
{%- assign today = today_date | date: '%s'| abs -%}
{%- assign beg_date = '2020-01-21' | date: '%s' | abs -%}
{%- assign beg_index = 0 -%}

{%- if today > beg_date -%}
  {%- assign end_index = site.data.schedule.weeks | size | minus: 2 -%}
  {%- for week in site.data.schedule.weeks limit:end_index -%}
    {%- assign first_day = week.columns | first -%}
    {%- if first_day.start -%}
      {%- assign as_seconds = first_day.start | date: '%s' | abs -%}
      {%- if as_seconds > today -%}
        {%- break -%}
      {%- endif -%}
    {%- endif -%}
    {%- assign beg_index = forloop.index0 -%}
  {%- endfor -%}
{%- endif -%}

{% for week in site.data.schedule.weeks offset:beg_index limit:2 %}
{% include week.html week = week %}
{% endfor %}
{% endcomment %}

## Google Calendar

Here is the combined calendar for this course, which includes the latest office hours schedule, upcoming deadlines, and more:

<iframe src="https://calendar.google.com/calendar/embed?height=600&amp;wkst=1&amp;bgcolor=%23ffffff&amp;ctz=America%2FLos_Angeles&amp;src=Y3MudXNmY2EuZWR1XzNnaDZiMmkybDM0cnNoNm1iY29zOHFyYXBnQGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20&amp;src=Y3MudXNmY2EuZWR1X200cGZ1Z2l2ZXM5ODI0c3ZtcWk5NHZ1Y2hrQGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20&amp;src=ZW4udXNhI2hvbGlkYXlAZ3JvdXAudi5jYWxlbmRhci5nb29nbGUuY29t&amp;src=OWRlMDFjYWo4NWMwdjFkZGpzb2pxZTU5NHFkZ3NyZjZAaW1wb3J0LmNhbGVuZGFyLmdvb2dsZS5jb20&amp;color=%23402175&amp;color=%2330487E&amp;color=%23515151&amp;color=%2330487E&amp;title=CS%20212&amp;showPrint=0&amp;showCalendars=0&amp;mode=WEEK" style="border-width:0; height: 600px;" width="100%" height="600" frameborder="0" scrolling="no"></iframe>

## Navigation

This website serves as the main portal for all content related to this course. To navigate this site:

<ul class="fa-ul" style="margin-left: 1in;">
{% for item in site.data.info.pages -%}
  <li>
  {% if item.icon -%}
    <span class="fa-li"><i class="{{ item.icon }}"></i></span>
  {% endif -%}
    <a href="{{ item.link | relative_url }}">{{ item.name }}</a>: {{ item.info }}
  </li>
{% endfor -%}
{% for values in site.data.info.links -%}
  {% assign label = values[0] -%}
  {% assign item = site.data.info.links[label] -%}
  <li {% if forloop.first %}class="bump"{% endif %}>
  {% if item.icon -%}
    <span class="fa-li"><i class="{{ item.icon }}"></i></span>
  {% endif -%}
    <a href="{{ item.link | relative_url }}">{{ item.name }}</a>: {{ item.info }}
  </li>
{% endfor -%}
</ul>

When in doubt, post on [Piazza]({{ site.data.info.links.piazza.link }}) for help finding content.
