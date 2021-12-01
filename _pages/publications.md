---
layout: page
permalink: /publications/
title: papers
description: Journal publications (IF only) in reverse chronological order starting with pre-prints.
years: [2022, 2021, 2020, 2019, 2017]
nav: true
---

Selected IF papers and pre-prints (submitted) only, for full list pleasee see my [scholar](https://scholar.google.pl/citations?user=z3bOMUAAAAAJ), [research-gate](https://www.researchgate.net/profile/Rafal-Kucharski-2) and [scopus](https://www.scopus.com/authid/detail.uri?authorId=57014903600).

<h2 class="pre-prints">pre-prints</h2>
  {% bibliography -f preprints}

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

