---
layout: splash
permalink: /
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/pk_header.png
excerpt: >
  A pair of professional software developers/hobbyist game developers creating games for fun and no profit.<br />
  <small><a href="/projects">Check out our Projects</a></small>
---
{% for post in site.posts limit:1 %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endfor %}
