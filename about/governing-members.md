---
title: Governing Members
layout: page-with-menu
---

The Engineering Society is run by volunteers in a wide variety of positions. It would be impossible to list everyone who contributes to its operation, but this page includes information about many of those volunteers. You can find all of their names and contact information below

## Officers

|Position|Officer|
|-|-|
|President|[Kenneth Lloyd Hilton](mailto:president@skule.ca)|
|Vice-President Finance|[Kelvin Lo](mailto:vpfinance@skule.ca)|
|Vice-President Communiciations|[Ethan Bhushan Mao](mailto:vpcomm@skule.ca)|
|Vice-President Academic|[Ziquan (Jim) Xu](mailto:vpacademic@skule.ca)|
|Vice-President Student Life|[Shosh Lebo](mailto:vpstudentlife@skule.ca)|
|Speaker|[Lavneet Singh](mailto:speaker@g.skule.ca)|
|Business Manager|[Rhonda Meek](mailto:rhonda@g.skule.ca)|

## Board of Directors

|Position|Representative|
|-|-|
|At-Large Representative|Binying (Edith) Fang|
|At-Large Representative|Valentina Lin Fang|
|At-Large Representative|Alyssa Tiw|
|At-Large Representative|*Vacant*|
|Chemical Engineering Representative|Jennifer Zhifeng Xu|
|Civil Engineering Representative|Dana Bou Saab|
|Electrical and Computer Engineering Representative|Justin Fang|
|Electrical and Computer Engineering Representative|*Vacant*|
|Engineering Science Representative|Elias Barsa|
|Industrial Engineering Representative|Jaden Benjamin Hinds|
|Mechanical Engineering Representative|Sebastian Kiernan|
|Materials Science and Engineering Representative|*Vacant*|
|Mineral Engineering Representative|*Vacant*|
|First Year Representative|Hankun Lin|
|First Year Representative|Jimmy Ji|
|First Year Representative|*Vacant*|

## Class Representatives

| Position | Representative |
| -------- | -------------- |

{% for discipline in site.data.council.reps %}
**{{ discipline[0] | upcase }}**  
{% assign years = discipline[1] %}
  {% for year in years %}
    {% assign year_label = year[0] | replace: "_", " " | capitalize %}
    {% assign people = year[1] %}
    
    {% if people == nil %}
      {# no reps here #}
    {% elsif people.size > 1 and people[0] %}
      {% comment %} people is an array {% endcomment %}
      {% for person in people %}
| {{ year_label }} | {{ person | markdownify | strip }} |
      {% endfor %}
    {% else %}
| {{ year_label }} | {{ people | markdownify | strip }} |
    {% endif %}
  {% endfor %}
{% endfor %}

