---
layout: about
title: about
permalink: /
subtitle: PhD Student, <a href="https://www.nankai.edu.cn/">Nankai University</a>

profile: false # enable when a personal profile photo is available

selected_papers: false # publications are displayed in the section below
social: false # enable after adding your own links to `_data/socials.yml`

announcements:
  enabled: false # enable after adding your own news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false # enable after adding your own blog posts
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I am a PhD student at [Nankai University](https://www.nankai.edu.cn/), advised by [Prof. Chongyi Li](https://li-chongyi.github.io/) and [Prof. Chun-Le Guo](https://guochunle-zero.github.io/).

My research focuses on **video super-resolution**.

Previously, I received my master's degree from [Beijing Union University](https://www.buu.edu.cn/), under the supervision of Prof. Mengmeng Zhang and Prof. Hongyuan Jing.

## Publications

_The entries below are fictional placeholders for layout preview and do not represent actual publications._

<div class="publications">

{% bibliography --group_by none --query @*[selected=true]* %}

</div>

[View all publications]({{ '/publications/' | relative_url }})

## Competitions and Awards

_The entries below are fictional placeholders for layout preview and do not represent actual achievements._

<ul>
  {% for award in site.data.awards %}
  <li>
    <strong>{{ award.year }} &mdash; {{ award.name | escape }}</strong><br>
    {{ award.result | escape }} &middot; {{ award.organizer | escape }} <em>(Placeholder)</em>
  </li>
  {% endfor %}
</ul>
