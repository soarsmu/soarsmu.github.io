---
title: "SOAR at SMU"
layout: gridlay
excerpt: "Allan Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

 **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**


Jump to [Staff and PhD Students](#staff), [Master and Bachelor Students](#master-and-bachelor-students), [Alumni](#alumni), [administrative support](#administrative-support), [lab visitors](#lab-visitors).

## Staff and PhD Students
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">

  {% if member.photo%}
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% endif %}


  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


## Current Master and Bachelor Students
<div class="row">

<div class="col-sm-6 clearfix">
<h4>Undergraduates</h4>
{% for member in site.data.bsc %}
{{ member.name }}
{% endfor %}
</div>

<div class="col-sm-6 clearfix">
<h4>Master students</h4>
{% for member in site.data.msc %}
{{ member.name }}
{% endfor %}
</div>


</div>

<!-- 
## Current Master and Bachelor Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %} -->


## Alumni



### Graduated PhD Students

* Lucia (Thesis: Ranking-Based Approaches for Localizing Faults)
Employment: Schroder Investment Management, Luxembourg
* <a href="https://sites.google.com/site/wswshaoweiwang/">Shaowei Wang</a> (Thesis: Multimodal Code Search)
Employment: Assistant Professor, Mississippi State University, USA
* <a href="http://sophiaytian.com/">Yuan Tian</a> (Thesis: Mining Bug Repositories for Automatic Software Bug Management: From Bug Triaging to Patch Backporting)
Employment: Assistant Professor, Queen’s University, Canada
* <a href="https://kochharps.wixsite.com/pavneet">Pavneet S. Kochhar</a> (Thesis: Testing and Debugging: A Reality Check)
Employment: Microsoft, Canada
* Tien-Duy B. Le (Thesis: Hybrid-Based Approaches for Software Fault Localization and Specification Mining)
Employment: Hudson River Trading, Singapore
* Ferdian Thung (Thesis: Recommending APIs for Software Evolution)
Employment: Research Scientist, SMU, Singapore
* <a href="https://xuanbachle.github.io">Xuan-Bach B. Le</a> (Thesis: Overfitting in Automated Program Repair: Challenges and Resolutions)
Employment: Lecturer (equiv. to Assistant Professor), University of Melbourne, Australia
* <a href="https://siqima.me">Siqi Ma</a> (Thesis: Automatic Vulnerability Detection and Repair; Co-Advisor)
Employment: Data 61, CSIRO, Australia
* <a href="https://abhishek9sharma.github.io">Abhishek Sharma</a> (Thesis: Social Software Development: Insights and Solutions)
Employment: Research Fellow, Living Analytics Research Center, Singapore
* Agus Sulistya (Thesis: Making Sense of Crowd-Generated Contents in Domain-Specific Settings)
Employment: Telkom, Indonesia

<!-- {% assign number_printed = 0 %}
{% for member in site.data.alumni_phds %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}



<div class="col-sm-6 clearfix">
  {% if member.photo%}
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% endif %}
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br> Thesis: {{ member.Thesis }} <br> Employment: {{member.employment}}</i>
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %} -->

### Former Postdocs

* <a href="https://baolingfeng.github.io">Lingfeng Bao</a> (Jun 2017 – Sep 2018)
Employment: Distinguished Researcher, Zhejiang University City College, China
* <a href="https://zhiyuan-wan.github.io">Zhiyuan Wan</a> (July – Dec 2018)
Employment: Postdoc, University of British Columbia, Canada
* Tien-Duy B. Le
Employment: Hudson River Trading, Singapore

<!-- {% assign number_printed = 0 %}
{% for member in site.data.alumni_postdocs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  {% if member.photo%}
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% endif %}
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br> Employment: {{member.employment}}</i>
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %} -->


###  Long-Term (1 year or longer) Visiting PhD Students (incomplete list):
* <a href="http://www.cs.utsa.edu/~xwang/">Xiaoyin Wang</a>, from Peking University, China (2008 –2009)
Employment: Associate Professor, University of Texas at San Antonio, USA
* <a href="https://xin-xia.github.io">Xin Xia</a>, from Zhejiang University, China (2012 –2014)
Employment: Lecturer (equiv. to Assistant Professor), Monash University, Australia
* Zhang Yun, from Zhejiang University, China
Employment: Associate Professor, Zhejiang University City College, China
* Weiqin Zou, from Nanjing University, China

### Short-Term Visiting PhD Students (incomplete list):
* <a href="https://bissyande.github.io">Tegawende Bissyande</a>, from University of Bordeaux, France (2012)
* <a href="https://le-an.gitlab.io">Le An</a>, from University of Montreal, Canada (2017)
* Xuan Huo, from Nanjing University, China (2018)
* Marcos Cesar de Oliveira, from University of Brasilia, Brazil (2018)



## Former Students
<div class="row">

<!-- <div class="col-sm-4 clearfix">
<h4>Visitors</h4>
{% for member in site.data.alumni_visitors %}
{{ member.name }}
{% endfor %}
</div> -->

<div class="col-sm-6 clearfix">
<h4>Bachelor Students</h4>
{% for member in site.data.alumni_bsc %}
{{ member.name }}
{% endfor %}
</div>

<div class="col-sm-6 clearfix">
<h4>Master students</h4>
{% for member in site.data.alumni_msc %}
{{ member.name }}
{% endfor %}
</div>

</div>


## Administrative Support
If you need to update your information, feel free to contact <a href="zyang@smu.edu.sg">Zhou YANG</a>.
