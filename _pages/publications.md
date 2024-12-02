---
title: "Publications"
layout: gridlay
sitemap: false
permalink: /publications/
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
{% bibliography --query @article %}
</div>

### Refereed conference proceedings
<div class="jumbotron">
{% bibliography --query @inproceedings %}
</div>
