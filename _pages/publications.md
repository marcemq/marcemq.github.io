---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

## Journals
{% for post in site.publications reversed %}
  {% if post.tags contains "journal" %}
      {% include archive-single-publi.html %}
  {% endif %}  
{% endfor %}

## Conferences
{% for post in site.publications reversed %}
  {% if post.tags contains "conference" %}
      {% include archive-single-publi.html %}
  {% endif %}  
{% endfor %}





