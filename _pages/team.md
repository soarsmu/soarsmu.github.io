---
title: "SOAR - Team"
layout: gridlay
excerpt: "SOftware Analytics Research Group -- Team Members"
sitemap: false
permalink: /team/
---

<h1 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">Team Members</h1>

## Faculty

<div class="row">
  <div class="col-sm-3 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/PhotoDLo-small.JPG" class="img-responsive" width="76%" style="float: center" />
  <br>
  <h4><a href="http://www.mysmu.edu/faculty/davidlo/">David Lo</a></h4>
  Professor<br>
  Lee Kuan Yew Fellow<br>
  <i><davidlo@smu.edu.sg></i><br>
  B.Eng (NTU), PhD (NUS)
  </div>

  <div class="col-sm-9"> 
  <p> David Lo is an <a href='https://www.acm.org/media-center/2019/october/distinguished-members-2019'>ACM Distinguished Member (Scientist)</a> and Professor of Information Systems at Singapore Management University, leading the Software Analytics Research (SOAR) group. His research interest is in the intersection of software engineering and data science, encompassing socio-technical aspects and analysis of different kinds of software artefacts, with the goal of improving software quality and developer productivity. <a href='https://dblp.uni-trier.de/pers/hd/l/Lo_0001:David'>His work</a> has been published in major and premier conferences and journals in the area of software engineering, AI, and cybersecurity attracting substantial <a href='https://scholar.google.com/citations?user=Ra4bt-oAAAAJ&hl=en'>interest</a> from the community. He has won more than 10 international research and service <a href='awards.html' target="middle">awards</a> including 6 ACM SIGSOFT Distinguished Paper awards. His work has been supported by <a href='https://www.nrf.gov.sg/'>NRF</a>, <a href='https://www.moe.gov.sg/'>MOE</a>, <a href='https://www.nrf.gov.sg/programmes/national-cybersecurity-r-d-programme'>NCR</a>, <a href='https://www.aisingapore.org/'>AI Singapore</a>, and several international research projects. He has served in more than 30 organizing committees and numerous program committees of research conferences including serving as general or program co-chairs of <a href="https://www.deakin.edu.au/ase2020" target="_blank">ASE 2020</a>, <a href="https://saner2019.github.io/" target="_blank">SANER 2019</a>, <a href='https://icsme2018.github.io/' target="_blank">ICSME 2018</a>, <a href='http://icpc2017.unibas.it/ ' target="_blank">ICPC 2017</a>, and <a href='http://www.ase2016.org/' target="_blank">ASE 2016<a>. He is also serving in the editorial board of <a href="https://www.computer.org/csdl/journal/ts" target="_blank">IEEE Transactions on Software Engineering</a>, <a href="http://www.springer.com/computer/programming/journal/10664" target="_blank">Empirical Software Engineering</a>, <a href="https://rs.ieee.org/publications/transactions-on-reliability.html" target="_blank">IEEE Transactions on Reliability</a>, <a href="http://onlinelibrary.wiley.com/journal/10.1002/(ISSN)2047-7481" target="_blank">Journal of Software: Evolution and Process</a>,  <a href="https://www.journals.elsevier.com/information-and-software-technology/" target="_blank">Information and Software Technology</a>, <a href="http://www.journals.elsevier.com/information-systems/" target="_blank">Information Systems</a>, and <a href="http://www.journals.elsevier.com/neurocomputing" target="_blank">Neurocomputing (Software Section)</a>. His former PhD students have secured faculty positions (University of Melbourne, Australia; Queen's University, Canada; Mississippi State University, USA; ITTelkom Surabaya, Indonesia) and employment at high-tech industries (Microsoft, Canada; Schroder Investment Management, Luxembourg; Hudson River Trading, Singapore; Veracode, Singapore) around the globe. </p>
  </div>
</div>


<div class="row">
  <div class="col-sm-3 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/Jiang.png" class="img-responsive" width="76%" style="float: center" />
  <br>
  <h4><a href="http://www.mysmu.edu/faculty/lxjiang/
  ">Lingxiao Jiang</a></h4>
  Associate Professor<br>
  <i><lxjiang@smu.edu.sg></i><br>
  B.Sc.,M.Sc., (Peking University), PhD (University of California)
  </div>

  <div class="col-sm-9"> 
  <p> Lingxiao Jiang is an Associate Professor of Information Systems at Singapore Management University. He worked as a test strategist at Nvidia for half a year before he joined the faculty of SCIS at SMU. He is broadly interested in the area of Software Engineering, Programming Languages, Systems, Security, and Data Mining. He has been spending substantial efforts on software mining, program analysis, code search & reuse, program comprehension & generation, aiming to provide practical techniques and tools for enhancing software reliability, increasing development productivity, reducing maintenance cost, and improving user experience. He received <a href="https://scis.smu.edu.sg/news/2018/nov/02/smu-researcher-wins-2018-acm-sigsoft-impact-paper-award">the 2018 ACM SIGSOFT Impact Paper Award</a>. The annual award is presented to authors of papers published at least ten years ago that have been deemed highly influential by the international software engineering community.
  A general theme of his work is mining and analysis for software engineering, such as detection of code clones, code query processing, detection of bugs, search for bug fixes, deep learning of code, and search for better testing & debugging techniques. The search is being carried out on various contextual data sources in addition to program code itself, such as code change histories, program bug databases, test suites, developer activities, user feedbacks, and socio-technical information pertaining to the complex interactions between people and technologies in both software development processes and real-world usage scenarios. To enable the extraction of information from various data sources and to enable efficient search and analysis, various technologies are being employed, such as static & dynamic program analysis, software engineering methodologies, data mining, machine learning, information retrieval, natural language processing, and distributed computing techniques. </p>
  </div>
</div>

**We are  looking for new PhD students, Postdocs, and Master students to join our team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies)**!**

<!-- Jump to [Research Staff and PhD Students](#research-staff-and-phd-students), [Master and Bachelor Students](#master-and-bachelor-students), [Alumni](#alumni), [administrative support](#administrative-support), [lab visitors](#lab-visitors). -->

## Research Staff and PhD Students
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
  {{ member.info }}<br>
  <i><{{ member.email }}></i>
  
  
  <ul class="fa-ul">

  {% if member.number_educ == 1 %}
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education1 }} </li>
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education1 }} </li>
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education2 }} </li>
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education1 }} </li>
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education2 }} </li>
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education3 }} </li>
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education1 }} </li>
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education2 }} </li>
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education3 }} </li>
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education4 }} </li>
    <li><img class="fa-li"><i class='fas fa-graduation-cap' style='font-size:13px;color:black'></i> {{ member.education5 }} </li>
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


<!-- ## Current Master and Bachelor Students -->
<div class="row">

<div class="col-sm-6 clearfix">
<h4>Undergraduates Students</h4>
{% for member in site.data.bsc %}
{{ member.name }}
{% endfor %}
</div>

<!-- <div class="col-sm-6 clearfix">
<h4>Master students</h4>
{% for member in site.data.msc %}
{{ member.name }}
{% endfor %}
</div> -->


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

<style>
  @media (max-width: 420px) {.fa-ul::before{content: "\A";white-space: pre;}}
</style>