---
title: "SOAR - Pictures"
layout: piclay
excerpt: "Allan Lab -- Pictures"
permalink: /pictures/
---

# Pictures



#### Gallery
(Right-click *'view image'* to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
<!-- <a>{{pic.title}}</a> -->
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>



<!-- ## SMU Campus

<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/SMU_SIS2.jpeg" width="60%">
</figure>

<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/SMU_SIS.jpeg" width="60%">
</figure>


## Animals in the Campus

<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/cat.jpeg" width="60%">
</figure>
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/cat2.jpeg" width="60%">
</figure> -->