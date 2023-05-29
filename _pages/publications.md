---
title: "SOAR - Publications"
layout: gridlay
excerpt: "SOftware Analytics Research Group -- Publications."
sitemap: false
permalink: /publications/
---

<h1 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">Selected Publications</h1>

(For a full list, please go to [DBLP](https://dblp.uni-trier.de/pers/hd/l/Lo_0001:David) or [Google Scholar](http://scholar.google.com/citations?user=Ra4bt-oAAAAJ&hl=en))

{% assign publications_by_year = site.data.publist | group_by: "year" | sort: "name" | reverse %}
{% for year in publications_by_year %}

### {{ year.name }}

{% assign publications = year.items | group_by: "type" | sort: "name" | reverse %}
{% for publication in publications %}

{% if publication.name == "Conference" %}
{% assign publi_type = "Conf" %}
{% else %}
{% assign publi_type = publication.name %}
{% endif %}

{% assign sorted_items = publication.items | sort: "publisher" %}
{% for item in sorted_items %}

<div class="col-sm-1" style="padding:0px">
  <div class="box {{publi_type}}"></div>
  <p style="display:inline-block;">[{{publi_type}}]</p>
</div>
<div class="col-sm-11">
<p>
**{{ item.title }}** <br/>
<em>{{ item.authors }} </em><br/>
{{ item.publisher }} ( {% if item.pdf %} <a href="/papers/2021/{{ item.pdf }}" target="_blank">Paper PDF</a> {% endif %} {% if item.pdf and item.doi %} | {% endif %} {% if item.doi %} <a href="{{ item.doi }}" target="_blank">DOI</a> {% endif %} {% if item.pdf and item.code %} | {% endif %} {% if item.code %} <a href="{{ item.code }}" target="_blank">Code</a> {% endif %} )
</p>
</div>
{% endfor %}
{% endfor %}
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

.Journal{
  background-color: #C32B72;
}
.Conf{
  background-color: #196CA3;
}
.Arxiv{
  background-color: #606B70;
}
.Editorship{
  background-color: #33C3BA;
}
</style>
