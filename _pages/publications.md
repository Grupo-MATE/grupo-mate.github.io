---
title: "Publications"
layout: gridlay
sitemap: false
permalink: /publications/
article_years: [2024,2023,2022,2021,2019,2018,2017,2016,2015,2013,2012,2011]
conference_years: [2024,2023,2022,2021,2020,2019,2018,2017,2016,2015,2014,2013,2012,2011,2010,2009,2008]
---

<style>
.jumbotron{
    padding:3%;
    padding-bottom:10px;
    padding-top:10px;
    margin-top:10px;
    margin-bottom:30px;
}
</style>

### Preprints
<div class="jumbotron">
{% bibliography --query @unpublished %}
</div>

### Refereed journal articles
<div class="jumbotron">
{% for y in page.article_years %}
<div class="text-right"> 
<h4 style="margin: 1em;"> {{ y }} </h4>
</div>

  {% bibliography -q @article[year={{y}}] %}
  
{% endfor %}

</div>

### Refereed conference proceedings
<div class="jumbotron">
{% for y in page.conference_years %}
<div class="text-right"> 
<h4 style="margin: 1em;"> {{ y }} </h4>
</div>

  {% bibliography -q @inproceedings[year={{y}}] %}
  
{% endfor %}

</div>