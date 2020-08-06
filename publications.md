---
title: Publications
permalink: /publications/
---

<h2>{{page.title}}</h2>
<br>
{% assign currentyear = 2020 %}

{% for year in (2010..currentyear) reversed %}
<div class="content list">
<h4>{{year}}</h4>
  {% for post in site.data.pub %}
    {% if post.year == year%}
    <div class="list-item">
    {% if post.image %}
      <a href="{{site.baseurl}}/{{post.pdf}}">
       <img src="{{site.baseurl}}/{{post.image}}" class="responsive-pub"
          alt="{{post.title}}" >
      </a>
    {%endif%}
    <p class="list-post-title" >
          {{ post.authors }} ({{ post.year }})
          {% if post.urlpaper %}
            <a href="{{post.urlpaper}}" style="color: #337cbb">{{ post.title }}</a>.
          {% else %}
            {{ post.title }}.
          {% endif %}
           <b>{{ post.journal }}.</b> {{post.pages}}.
           {% if post.pdf %}<a href="{{site.baseurl}}/{{post.pdf}}" style="color: #337cbb"><b>[PDF]</b></a>{% endif %}
           {% if post.note %} <i style="color: #337cbb"> ({{post.note}}) </i> {% endif %}
    </p>
    <br style="clear:both" />
    </div>

    {% endif%}
  {% endfor %}
</div><br>
{% endfor %}



### Copyright Notice

This material is presented to ensure timely dissemination of scholarly and technical work. All documents are author's copy of accepted manuscripts. Copyright and all rights
therein are retained by authors or by other copyright holders. All persons copying this information are expected to adhere to the terms and constraints invoked by each author's copyright. In most cases, these works may not be reposted without the explicit permission of the copyright holder.
