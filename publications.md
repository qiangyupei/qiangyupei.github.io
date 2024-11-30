---
layout: page
title: "Publications"
permalink: /publications/
main_nav: true
---

<!-- All Publications-->
<h3>Conference Publications</h3>
<ul class="pub-list-style">
  {% for publication in site.data.publications_conference %}
  <li>
    <span class="conference-name">{{ publication.conference }}</span>
    {% assign authors = publication.authors | split: ', ' %}
    {% for author in authors %}
      {% if author == "Qiangyu Pei" %}
        <strong>{{ author }}</strong>{% if forloop.last == false %},{% endif %}
      {% else %}
        {{ author }}{% if forloop.last == false %},{% endif %}
      {% endif %}
    {% endfor %}
    {% if publication.link_type == "file" %}<a href="{{ '/files/' | append: publication.link }}" target="_blank" rel="noopener noreferrer">{{ publication.title }}</a>{% elsif publication.link_type == "external" %}<a href="{{ publication.link }}" target="_blank" rel="noopener noreferrer">{{ publication.title }}</a>{% endif %}{% if publication.extra_file and publication.extra_file_name %}, <a href="{{ '/files/' | append: publication.extra_file }}" target="_blank" rel="noopener noreferrer">{{ publication.extra_file_name }}</a>{% endif %}
  </li>
  {% endfor %}
</ul>

<h3>Journal Publications</h3>
<ul class="pub-list-style2">
  {% for publication in site.data.publications_journal %}
  <li>
    <strong>[{{ publication.conference }}]</strong>&nbsp;
    {% assign authors = publication.authors | split: ', ' %}
    {% for author in authors %}
      {% if author == "Qiangyu Pei" %}
        <strong>{{ author }}</strong>{% if forloop.last == false %},{% endif %}
      {% else %}
        {{ author }}{% if forloop.last == false %},{% endif %}
      {% endif %}
    {% endfor %}
    {% if publication.link_type == "file" %}<a href="{{ '/files/' | append: publication.link }}" target="_blank" rel="noopener noreferrer">{{ publication.title }}</a>{% elsif publication.link_type == "external" %}<a href="{{ publication.link }}" target="_blank" rel="noopener noreferrer">{{ publication.title }}</a>{% endif %}{% if publication.extra_file and publication.extra_file_name %}, <a href="{{ '/files/' | append: publication.extra_file }}" target="_blank" rel="noopener noreferrer">{{ publication.extra_file_name }}</a>{% endif %}
  </li>
  {% endfor %}
</ul>