<!-- ---
layout: page
title: "Blog"
permalink: /blogs/
main_nav: true
--- -->

{% for category in site.categories %}
  {% capture cat %}{{ category | first }}{% endcapture %}
  <h2 id="{{cat}}">{{ cat | capitalize }}</h2>
  {% for desc in site.descriptions %}
    {% if desc.cat == cat %}
      <p class="desc"><em>{{ desc.desc }}</em></p>
    {% endif %}
  {% endfor %}
  <ul class="blogs-list">
  {% for blog in site.categories[cat] %}
    <li>
      <strong>
        <a href="{{ blog.url | prepend: site.baseurl }}">{{ blog.title }}</a>
      </strong>
      <span class="blog-date">- {{ blog.date | date_to_long_string }}</span>
    </li>
  {% endfor %}
  </ul>
  {% if forloop.last == false %}<hr>{% endif %}
{% endfor %}
<br>
