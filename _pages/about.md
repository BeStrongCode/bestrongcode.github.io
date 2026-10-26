---
layout: default
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
  </figure>
  <div class="about-biography" style="flex: 1 1 320px; min-width: 0;">
    <header class="about-identity" style="margin: 0 0 1.25rem;">
      <h1 style="margin: 0; font-size: 2rem; line-height: 1.2; font-weight: 600;">{{ site.first_name | escape }} {{ site.last_name | escape }}</h1>
      <p style="margin: 0.4rem 0 0; font-size: 1rem; line-height: 1.5;">{{ page.subtitle }}</p>
    </header>
    <p>
      I am a PhD student at <a href="https://www.nankai.edu.cn/">Nankai University</a>, advised by
      <a href="https://li-chongyi.github.io/">Prof. Chongyi Li</a> and <a href="https://guochunle-zero.github.io/">Prof. Chun-Le Guo</a>.
    </p>
    <p>
      Previously, I received my master's degree from <a href="https://www.buu.edu.cn/">Beijing Union University</a>, under the supervision of
      <a href="https://baike.baidu.com/item/%E5%BC%A0%E8%90%8C%E8%90%8C/3998470?fr=aladdin/"> Prof. Mengmeng Zhang </a>and <a href="https://graduate.buu.edu.cn/art/2026/3/1/art_30716_822945.html/"> Prof. Hongyuan Jing.
    </p>
    <p>My research focuses on <strong>video super-resolution</strong>.</p>
  </div>
</div>

## Publications

<link rel="stylesheet" href="{{ '/assets/css/personal-publications.css' | relative_url }}">

<div class="publications">

{% bibliography --group_by none --query @*[selected=true]* %}

</div>

[View all publications]({{ '/publications/' | relative_url }})

## Competitions and Awards

<ul class="awards-list">
  {% for award in site.data.awards %}
  <li>
    {% if award.category == 'competition' %}
    <strong><span class="award-highlight">{{ award.result | escape }}</span> of {{ award.name | escape }}</strong>{% if award.role %}
    <span class="award-highlight">({{ award.role | escape }})</span>{% endif %}
    {% else %}
    <strong>{{ award.year }} &mdash; {{ award.name | escape }}</strong><br>
    {{ award.result | escape }}
    {% endif %}
  </li>
  {% endfor %}
</ul>
