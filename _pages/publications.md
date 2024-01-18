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

{% for post in site.publications reversed %}
  <h2 onclick="window.location='{{ post.permalink }}'" style="cursor:pointer; color: blue; text-decoration: underline;">{{ post.title }}</h2>
  <p><strong>Authors:</strong> {{ post.authors }}</p>
  <p><strong>Paper URL:</strong> <a href="{{ Download here }}">{{ post.paperurl }}</a></p>
  <!-- Add more details as needed -->

{% endfor %}