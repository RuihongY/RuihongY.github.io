---
layout: paper
title: "Publications"
permalink: /publications/
equal_note: true
---

{% include base_path %}

{% for category in site.publication_category reversed %}
{% assign posts = site.publications | where: "category", category[0] | sort: "date" | reverse %}
{% if posts.size > 0 %}
<h2>{{ category[1].title }}</h2>
{% for post in posts %}
<section class="entry">
  <h3><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></h3>
  <p class="citation">{{ post.authors | append: "." | replace: "..", "." | replace: "R. Yin", "<b>R. Yin</b>" }} <i>{{ post.venue }}</i> ({{ post.date | date: "%Y" }}).</p>
  <div class="abstract">{{ post.content }}</div>
</section>
{% endfor %}
{% endif %}
{% endfor %}
