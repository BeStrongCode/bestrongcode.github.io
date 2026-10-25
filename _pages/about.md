---
layout: about
title: about
permalink: /
subtitle: PhD Student, <a href="https://www.nankai.edu.cn/">Nankai University</a>

profile: false # the portrait and biography are arranged together below

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

<div class="about-intro" style="display: flex; flex-wrap: wrap; align-items: flex-start; gap: 2rem; margin-bottom: 2rem;">
  <figure style="flex: 0 0 200px; width: 200px; max-width: 100%; margin: 0 auto;">
    <img
      src="{{ '/assets/img/rqy.jpg' | relative_url }}"
      alt="Portrait of Qiyu Rong"
      width="1050"
      height="1350"
      style="display: block; width: 100%; height: auto; border-radius: 0.5rem;"
    >
    <figcaption style="margin-top: 0.75rem; text-align: center; font-size: 1.25rem; font-weight: 600;">
      {{ site.first_name | escape }} {{ site.last_name | escape }}
    </figcaption>
  </figure>
  <div class="about-biography" style="flex: 1 1 320px; min-width: 0;">
    <p>
      I am a PhD student at <a href="https://www.nankai.edu.cn/">Nankai University</a>, advised by
      <a href="https://li-chongyi.github.io/">Prof. Chongyi Li</a> and <a href="https://guochunle-zero.github.io/">Prof. Chun-Le Guo</a>.
    </p>
    <p>
      Previously, I received my master's degree from <a href="https://www.buu.edu.cn/">Beijing Union University</a>, under the supervision of
      Prof. Mengmeng Zhang and Prof. Hongyuan Jing.
    </p>
    <p>My research focuses on <strong>video super-resolution</strong>.</p>
  </div>
</div>

## Publications

_The entries below are fictional placeholders for layout preview and do not represent actual publications._

<div class="publications">

{% bibliography --group_by none --query @*[selected=true]* %}

</div>

[View all publications]({{ '/publications/' | relative_url }})

## Competitions and Awards

<ul>
  {% for award in site.data.awards %}
  <li>
    <strong>{{ award.year }} &mdash; {{ award.name | escape }}</strong><br>
    {{ award.result | escape }}{% if award.role %} ({{ award.role | escape }}){% endif %}
  </li>
  {% endfor %}
</ul>
