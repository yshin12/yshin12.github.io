---
title:  "Research"
layout: archive
permalink: /research/
author_profile: true
comments: false
classes: wide
---




## Publications

<ol>
{% for paper in site.data.papers.papers %}
  <li>
      {% if paper.title %}<b>{{ paper.title }}</b>, {% endif %}
      {% if paper.coauthors %} (with {{ paper.coauthors }}), {% endif %}
      {% if paper.journal %} <span style="font-style: italic; color:#000099">{{ paper.journal }},</span> {% endif %}
      {% if paper.vol_no %} {{ paper.vol_no }}, {% endif %}
      {% if paper.year %} 
        {% if paper.page %} 
            {{ paper.year }}, pp. {{ paper.page }}
        {% else %}
            {{ paper.year }} 
        {% endif %} 
      {% endif %}
      {% if paper.link %}<a href="{{ paper.link }}"  target="_blank">{{ "[journal]" }}</a> {% endif %}
      {% if paper.arxiv %}<a href="{{ paper.arxiv }}" target="_blank">{{ "[arXiv]" }}</a>{% endif %}
  </li>
{% endfor %} 
</ol>



## Working Papers
<ol>
{% for paper in site.data.papers.workingpapers %}
  <li>
      {% if paper.title %}<b>{{ paper.title }}</b>, {% endif %}
      {% if paper.coauthors %} (with {{ paper.coauthors }}), {% endif %}
      {% if paper.vol_no %} {{ paper.vol_no }}, {% endif %}
      {% if paper.journal %} <span style="font-style: italic; color:#000099">{{ paper.journal }},</span> {% endif %}
      {% if paper.year %} {{ paper.year }} {% endif %}
      {% if paper.link %}<a href="{{ paper.link }}"  target="_blank">{{ "[journal]" }}</a> {% endif %}
      {% if paper.arxiv %}<a href="{{ paper.arxiv }}" target="_blank">{{ "[arXiv]" }}</a>{% endif %}
  </li>
{% endfor %}
</ol>
