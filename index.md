---
layout: archive
author_profile: true
title: " "
classes: wide
---


## Research Interests
- Causal inference and identification
- Modern computational algorithm and inference
- Applications of statistical decision theory

## Recent Publications
{% for paper in site.data.papers.papers %}
  {% if forloop.index < 6 %}
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
  {% endif %}
{% endfor %} 



## Recent Working Papers
{% for paper in site.data.papers.workingpapers %}
  {% if forloop.index < 5 %}
  <li>
	  {% if paper.title %}<b>{{ paper.title }}</b>, {% endif %}
      {% if paper.coauthors %} (with {{ paper.coauthors }}), {% endif %}
      {% if paper.vol_no %} {{ paper.vol_no }}, {% endif %}
      {% if paper.journal %} <span style="font-style: italic; color:#000099">{{ paper.journal }},</span> {% endif %}
      {% if paper.year %} {{ paper.year }} {% endif %}
      {% if paper.link %}<a href="{{ paper.link }}"  target="_blank">{{ "[journal]" }}</a> {% endif %}
	  {% if paper.arxiv %}<a href="{{ paper.arxiv }}" target="_blank">{{ "[arXiv]" }}</a>{% endif %}
  </li>
  {% endif %}
{% endfor %}


A full list of my research papers is available at [Research](/research/). A pdf file of my curriculum vitae can be downloaded from [CV](/assets/pdf/youngkiCV.pdf).

Updated: November 8, 2022.



