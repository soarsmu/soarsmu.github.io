---
title: "SOAR - Publications"
layout: gridlay
excerpt: "SOAR -- Publications."
sitemap: false
permalink: /publications/
---


# Publications
<!-- 
## Group highlights

(For a full list see [below](#full-list) or go to [DBLP](https://dblp.uni-trier.de/pers/hd/l/Lo_0001:David), [Google Scholar](http://scholar.google.com/citations?user=Ra4bt-oAAAAJ&hl=en))

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>

## Full List
 -->

(For a full list, please go to [DBLP](https://dblp.uni-trier.de/pers/hd/l/Lo_0001:David) or [Google Scholar](http://scholar.google.com/citations?user=Ra4bt-oAAAAJ&hl=en))

### 2020

{% for publi in site.data.publist_2020 %}

  {{ publi.title }} <br/>
  <em>{{ publi.authors }} </em><br/>
  {{ publi.publisher }} ({% if publi.pdf %} <a href="/papers/2020/{{ publi.pdf }}" target="_blank">Paper PDF</a> {% endif %} {% if publi.bib %} | <a href="{{ publi.bib }}" target="_blank">BIB</a> {% endif %} {% if publi.code %} | <a href="{{ publi.code }}" target="_blank">Code</a> {% endif %} )
  
{% endfor %}

### 2019

{% for publi in site.data.publist_2019 %}

  {{ publi.title }} <br/>
  <em>{{ publi.authors }} </em><br/>
  {{ publi.publisher }} ( {% if publi.pdf %} <a href="/papers/2019/{{ publi.pdf }}" target="_blank">Paper PDF</a> {% endif %} {% if publi.bib %} | <a href="{{ publi.bib }}" target="_blank">BIB</a> {% endif %} {% if publi.code %} | <a href="{{ publi.code }}" target="_blank">Code</a> {% endif %} )
  
{% endfor %}
