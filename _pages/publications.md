---
title: "SOAR - Publications"
layout: gridlay
excerpt: "SOftware Analytics Research Group -- Publications."
sitemap: false
permalink: /publications/
---


<h1 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">Publications</h1>
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

<div class="col-sm-1" style="padding:0px">
  {% if publi.type == "Journal" %} 
  <div class="box" style="background-color: #C32B72;"></div>
  <p style="display:inline-block;">[Journal] </p>
  {% endif %}
  {% if publi.type == "Conference" %} 
  <div class="box" style="background-color: #196CA3;"></div>
  <p style="display:inline-block;">[Conf] </p>
  {% endif %}
  {% if publi.type == "Arxiv" %} 
  <div class="box" style="background-color: #606B70;"></div>
  <p style="display:inline-block;">[Arxiv] </p>
  {% endif %}
  {% if publi.type == "Editorship" %} 
  <div class="box" style="background-color: #33C3BA;"></div>
  <p style="display:inline-block;">[Editor] </p>
  {% endif %}
  {% if publi.type <> "Journal" and publi.type <> "Conference" and publi.type <> "Arxiv" and publi.type <> "Editorship" %} 
  <div class="box"></div>
  <p style="display:inline-block;">[Other] </p>
  {% endif %}
</div>
<div class="col-sm-11">
  <p>
  **{{ publi.title }}** <br/>
  <em>{{ publi.authors }} </em><br/>
  {{ publi.publisher }} ( {% if publi.pdf %} <a href="/papers/2020/{{ publi.pdf }}" target="_blank">Paper PDF</a> {% endif %} {% if publi.pdf and publi.bib %} | {% endif %} {% if publi.bib %} <a href="{{ publi.bib }}" target="_blank">BIB</a> {% endif %} {% if publi.pdf and publi.code %} | {% endif %}  {% if publi.code %} <a href="{{ publi.code }}" target="_blank">Code</a> {% endif %} )
  </p>
</div>

{% endfor %}


### 2019

{% for publi in site.data.publist_2019 %}

<div class="col-sm-1" style="padding:0px">
  {% if publi.type == "Journal" %} 
  <div class="box" style="background-color: #C32B72;"></div>
  <p style="display:inline-block;">[Journal] </p>
  {% endif %}
  {% if publi.type == "Conference" %} 
  <div class="box" style="background-color: #196CA3;"></div>
  <p style="display:inline-block;">[Conf] </p>
  {% endif %}
  {% if publi.type == "Arxiv" %} 
  <div class="box" style="background-color: #606B70;"></div>
  <p style="display:inline-block;">[Arxiv] </p>
  {% endif %}
  {% if publi.type == "Editorship" %} 
  <div class="box" style="background-color: #33C3BA;"></div>
  <p style="display:inline-block;">[Editor] </p>
  {% endif %}
  {% if publi.type <> "Journal" and publi.type <> "Conference" and publi.type <> "Arxiv" and publi.type <> "Editorship" %} 
  <div class="box"></div>
  <p style="display:inline-block;">[Other] </p>
  {% endif %}
</div>
<div class="col-sm-11">
  <p>
  **{{ publi.title }}** <br/>
  <em>{{ publi.authors }} </em><br/>
  {{ publi.publisher }} ( {% if publi.pdf %} <a href="/papers/2019/{{ publi.pdf }}" target="_blank">Paper PDF</a> {% endif %} {% if publi.pdf and publi.bib %} | {% endif %} {% if publi.bib %} <a href="{{ publi.bib }}" target="_blank">BIB</a> {% endif %} {% if publi.pdf and publi.code %} | {% endif %}  {% if publi.code %} <a href="{{ publi.code }}" target="_blank">Code</a> {% endif %} )
  </p>
</div>

{% endfor %}

### 2018

{% for publi in site.data.publist_2018 %}

<div class="col-sm-1" style="padding:0px">
  {% if publi.type == "Journal" %} 
  <div class="box" style="background-color: #C32B72;"></div>
  <p style="display:inline-block;">[Journal] </p>
  {% endif %}
  {% if publi.type == "Conference" %} 
  <div class="box" style="background-color: #196CA3;"></div>
  <p style="display:inline-block;">[Conf] </p>
  {% endif %}
  {% if publi.type == "Arxiv" %} 
  <div class="box" style="background-color: #606B70;"></div>
  <p style="display:inline-block;">[Arxiv] </p>
  {% endif %}
  {% if publi.type == "Editorship" %} 
  <div class="box" style="background-color: #33C3BA;"></div>
  <p style="display:inline-block;">[Editor] </p>
  {% endif %}
  {% if publi.type <> "Journal" and publi.type <> "Conference" and publi.type <> "Arxiv" and publi.type <> "Editorship" %} 
  <div class="box"></div>
  <p style="display:inline-block;">[Other] </p>
  {% endif %}
</div>
<div class="col-sm-11">
  <p>
  **{{ publi.title }}** <br/>
  <em>{{ publi.authors }} </em><br/>
  {{ publi.publisher }} ( {% if publi.pdf %} <a href="/papers/2018/{{ publi.pdf }}" target="_blank">Paper PDF</a> {% endif %} {% if publi.pdf and publi.bib %} | {% endif %} {% if publi.bib %} <a href="{{ publi.bib }}" target="_blank">BIB</a> {% endif %} {% if publi.pdf and publi.code %} | {% endif %}  {% if publi.code %} <a href="{{ publi.code }}" target="_blank">Code</a> {% endif %} )
  </p>
</div>

{% endfor %}

<style>
.container {
  height: 200px;
  position: relative;
  border: 3px solid green;
}

.vertical-center {
  margin: 0;
  position: absolute;
  top: 50%;
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
}

.box {
  display:inline-block;
  width:8px;
  height:8px;
  background-color: grey;
  margin-right:6px;
}
</style>
