---
layout: page
title: grants
permalink: /projects/
descr---
layout: page
title: projects
permalink: /projects/
description: A growing collection of your cool projects.
nav: true
display_categories: [work, fun]
horizontal: false
---
<div class="projects">
  {% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
    {% for category in page.display_categories %}
      <h2 class="category">{{ category }}</h2>
      {% assign categorized_projects = site.projects | where: "category", category %}
      {% assign sorted_projects = categorized_projects | sort: "importance" %}
      <!-- Generate cards for each project -->
      {% if page.horizontal %}
        <div class="container">
          <div class="row row-cols-2">
          {% for project in sorted_projects %}
            {% include projects_horizontal.html %}
          {% endfor %}
          </div>
        </div>
      {% else %}
        <div class="grid">
          {% for project in sorted_projects %}
            {% include projects.html %}
          {% endfor %}
        </div>
      {% endif %}
    {% endfor %}

  {% else %}
  <!-- Display projects without categories -->
    {% assign sorted_projects = site.projects | sort: "importance" %}
    <!-- Generate cards for each project -->
    {% if page.horizontal %}
      <div class="container">
        <div class="row row-cols-2">
        {% for project in sorted_projects %}
          {% include projects_horizontal.html %}
        {% endfor %}
        </div>
      </div>
    {% else %}
      <div class="grid">
        {% for project in sorted_projects %}
          {% include projects.html %}
        {% endfor %}
      </div>
    {% endif %}

  {% endif %}

</div>
iption: On-going externally-funded research projects
nav: true
---

We run several on-going externally-funded research projects:


### 1. Post-corona shared mobility

> Modelling and controlling virus spread processes in shared mobility networks 2021-2024, 1mln PLN funded by National Science Centre under scheme OPUS 19, funding 2PhD Positions and PostDoc
---



We anticipate substantial changes to post-corona urban mobility, when safety concerns will drive individual,
as well as, public decision makers. Travellers’ choices are likely to shift towards modes of low exposure to viruses.
Consequently, the sustainable mobility paradigm needs to drift into ’sustainable, yet safe’, unleashing a novel
trade-off dilemmas spanned between: cost-comfort-safety for individuals and: sustainability-efficiency-safety
for policymakers. Outcomes of those decision patterns are likely to disturb landscape of urban mobility. When
sustainable mass transit modes start being avoided by risk averse travellers, it may have devastating consequences
on performance of transport systems (congestion and traffic delays) and its externalities (emissions, pressure
on public space, etc.), which shall be counteracted.
Notably, due to recent, disruptive changes in urban mobility, the, so-called, shared mobility (where two or
more travellers share the same vehicle to reach the destination), provided via two-sided platforms (like Uber
and Lyft), has proven to be an appealing alternative. Whether it will remain attractive solution for emerging
mobility problems remains unknown. In particular, it is not known: a) how travellers willingness-to-share will
change b) how viruses spread through the shareability graph c) how can we redesign shared rides system to
control spreading and make sharing rides safe. This calls for a new set of models, theories and analyses to
understand how shared rides can contribute to post-corona urban mobility. To this end, in this project we aim to:

* WP1:forecast demand for post-corona shared mobility Data-driven travel behaviour
modelling. Series of stated preference experiments to estimate the post-corona willingness-to-share
among the virus-aware travellers. Predict a presumably non-deterministic, heterogeneous
travellers’ reaction to applied measures and virus exposure.

* WP2: model virus spreading on shared mobility networks Epidemic simulations with
stochastic, time evolving contact networks. Reproduce and understand contact networks
emerging from shared mobility to better model and predict spreading processes. Analyse
structure of underlying network connectivity and identify hubs, communities, size and depth
of diffusion trees and giant components.

* WP3: propose efficient strategies to trace and control it
Control, trace and halt spreading with a proactive strategic, tactical and operational system
management to make sharing safe again. Demand management to keep system attractive, yet
controlling the contact to prevent a future outbreaks.

Two PhD students involved: Michal Bujak and Farnoud Ghasemi


----
### 2. DigiWorld - Strategic Program Excellence Initiative at Jagiellonian University 
> Fully funded tenure-track professor position at Group of Machine Learning

With this grant I enjoy a three-year fully funded assistant professor position to collaborate with Group of Machine Learning af Faculty of Mathematics.
We explore intersections between AI/ML and modern ubran mobility. 
We employ Reinforcement Learning, Graph Neural Networks and Deep Learning to solve urban mobility problems (flow, speed, route, demand, etc.).
We are opened for (potentially funded) Master Student projects - see active opened projects (here)[https://gmum.net/]

---


