<!-- ---
layout: page
title: "Publication"
permalink: /files/
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
  <ul class="files-list">
  {% for file in site.categories[cat] %}
    <li>
      <strong>
        <a href="{{ file.url | prepend: site.baseurl }}">{{ file.title }}</a>
      </strong>
      <span class="file-date">- {{ file.date | date_to_long_string }}</span>
    </li>
  {% endfor %}
  </ul>
  {% if forloop.last == false %}<hr>{% endif %}
{% endfor %}
<br>
