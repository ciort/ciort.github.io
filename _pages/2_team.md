---
layout: page
title: team
permalink: /team/
description: Research group
nav: true
---


Our *group* targets at interesction of urban mobility and machine learning. We are interested in complex systems of urban mobility, specifically emerging modes, like **two-sided platforms and ride pooling**. Currently, we have are group of four: 2PhDs, one PD, PI. We are based in Krakow, Poland at Jagiellonian University Campus (Krakow, prof. Lojasiewicza 6 [here](https://goo.gl/maps/K6c3wY7Zx3c1Jq9k6)


<div class="team">
  {% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
    {% for category in page.display_categories %}
      <h2 class="category">{{ category }}</h2>
      {% assign categorized_projects = site.team | where: "category", category %}
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
    {% assign sorted_projects = site.team | sort: "importance" %}
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


  
  
----
# Alumni

## PhD Students
* [Akradiusz Drabicki](https://www.researchgate.net/profile/Arkadiusz-Drabicki) - co-supervised by prof. Oded Cats (TU Delft) and prof. Andrzej Szarata (CUT Krakow). Arek researched a novel and emerging research field - he tried to understand the impacts of futuristic RTCI: Real-time crowding information for Public Transport. He extended and developed new functionalities to BusMezzo and ended-up with remarkable stream of publications marking the new territory in Public Transport see scholar [here](https://scholar.google.pl/citations?user=-XyYxkoAAAAJ). Expected graduation 2021/2022.

* Also, I co-laborated, yet did not supervised 4 PhD students of [Critical MaaS](http://smartptlab.tudelft.nl/projects/criticalmaas) project in TU Delft: Arjan de Ruijter ([his project](http://smartptlab.tudelft.nl/our-group/arjan-de-ruijter) ), Nejc Gerzinic ([his project](http://smartptlab.tudelft.nl/our-group/nejc-gerzinic)), Subodh Dubey and Peyman Ashkrof - with some I co-authored papers, for some I developed software for the needs of the thesis, yet they were not formally supervised by me.

## Master/undergrad students

here I will list only new students (2021-...), prior 2021 over 20 MA and undergrad students graduated with me at Cracow University of Technology

* Marco Maricic _The effects of pricing and service configurations on a ride-pooling service with pick-up and drop-off points_ - **TU Delft 2021** [thesis](https://repository.tudelft.nl/islandora/object/uuid%3A3e9426a7-a3ec-4943-af7c-55a26592beaa)
* Daan Knobe _IMPACT OF EMPTY TAXI REPOSITIONING STRATEGIES ON RIDESOURCING SYSTEM PERFORMANCE_ - **TU Delft, 2021**
* Farnoud Ghasemi _Ride acceptance behaviour investigation of ride-sourcing drivers through agent-based model_ - **La Sapienza, Rome, 2021**



---








