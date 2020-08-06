---
title: News
permalink: /news/
---

<h2>{{page.title}}</h2>
<br>
<p></p>

{% for news in site.data.news %}
  <p> <font color="#268bd2"> {{ news.date }}</font> - {{ news.description | markdownify | remove: '<p>' | remove: '</p>'  }}
  <br>
  </p>
{% endfor %}
