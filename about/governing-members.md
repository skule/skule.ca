---
title: Governing Members
layout: page-with-menu
---

The Engineering Society is run by volunteers in a wide variety of positions. It would be impossible to list everyone who contributes to its operation, but this page includes information about many of those volunteers. You can find all of their names and contact information below

## Officers

|Position|Officer|
|-|-|
|President|[{{ site.data.council.officer.president }}](mailto:president@skule.ca)|
|Vice-President Finance|[{{ site.data.council.officer.vp_finance }}](mailto:vpfinance@skule.ca)|
|Vice-President Communications|[{{ site.data.council.officer.vp_communications }}](mailto:vpcomm@skule.ca)|
|Vice-President Academic|[{{ site.data.council.officer.vp_academic }}](mailto:vpacademic@skule.ca)|
|Vice-President Student Life|[{{ site.data.council.officer.vp_student_life }}](mailto:vpstudentlife@skule.ca)|
|Speaker|[{{ site.data.council.officer.speaker }}](mailto:speaker@g.skule.ca)|
|Business Manager|[{{ site.data.council.officer.business_manager }}](mailto:rhonda@g.skule.ca)|

## Board of Directors

|Position|Representative|
|-|-|
{% for rep in site.data.council.bod_representatives.at_large %}|At-Large Representative|{{ rep }}|
{% endfor %}|Chemical Engineering Representative|{{ site.data.council.bod_representatives.chemical }}|
|Civil Engineering Representative|{{ site.data.council.bod_representatives.civil }}|
{% for rep in site.data.council.bod_representatives.ece %}|Electrical and Computer Engineering Representative|{{ rep }}|
{% endfor %}|Engineering Science Representative|{{ site.data.council.bod_representatives.engsci }}|
|Industrial Engineering Representative|{{ site.data.council.bod_representatives.industrial }}|
|Mechanical Engineering Representative|{{ site.data.council.bod_representatives.mechanical }}|
|Materials Science and Engineering Representative|{{ site.data.council.bod_representatives.mse }}|
|Mineral Engineering Representative|{{ site.data.council.bod_representatives.mineral }}|
{% for rep in site.data.council.bod_representatives.first_year %}|First Year Representative|{{ rep }}|
{% endfor %}

## Class Representatives

|Position|Representative|
|-|-|
{% for year in site.data.council.reps %}
|**{{ year[0] | replace: "_", " " | capitalize }}**||
{% for discipline in year[1] %}
  {% assign reps = discipline[1] %}
  {% if reps %}
    {% if reps.first %}
      {% for rep in reps %}|{{ discipline[0] | capitalize }}|{{ rep }}|
      {% endfor %}
    {% else %}
      |{{ discipline[0] | capitalize }}|{{ reps }}|
    {% endif %}
  {% endif %}
{% endfor %}
{% endfor %}
