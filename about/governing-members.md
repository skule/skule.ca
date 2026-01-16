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
|First Year|{{ site.data.council.reps.first_year.chemical }}|
|Second Year|{{ site.data.council.reps.second_year.chemical }}|
|Third Year|{{ site.data.council.reps.third_year.chemical }}|
|PEY|{{ site.data.council.reps.pey.chemical }}|
|Fourth Year|{{ site.data.council.reps.fourth_year.chemical }}|

|**Civil**||
|First Year|{{ site.data.council.reps.first_year.civil }}|
|Second Year|{{ site.data.council.reps.second_year.civil }}|
|Third Year|{{ site.data.council.reps.third_year.civil }}|
{% for rep in site.data.council.reps.pey.civil %}|PEY|{{ rep }}|
{% endfor %}|Fourth Year|{{ site.data.council.reps.fourth_year.civil }}|

|**ECE**||
{% for rep in site.data.council.reps.first_year.ece %}|First Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.second_year.ece %}|Second Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.third_year.ece %}|Third Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.pey.ece %}|PEY|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.fourth_year.ece %}|Fourth Year|{{ rep }}|
{% endfor %}

|**EngSci**||
{% for rep in site.data.council.reps.first_year.engsci %}|First Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.second_year.engsci %}|Second Year|{{ rep }}|
{% endfor %}|Third Year|{{ site.data.council.reps.third_year.engsci }}|
|PEY|{{ site.data.council.reps.pey.engsci }}|
|Fourth Year|{{ site.data.council.reps.fourth_year.engsci }}|

|**Industrial**||
{% for rep in site.data.council.reps.first_year.industrial %}|First Year|{{ rep }}|
{% endfor %}|Second Year|{{ site.data.council.reps.second_year.industrial }}|
|Third Year|{{ site.data.council.reps.third_year.industrial }}|
|PEY|{{ site.data.council.reps.pey.industrial }}|
|Fourth Year|{{ site.data.council.reps.fourth_year.industrial }}|

|**MSE**||
|First Year|{{ site.data.council.reps.first_year.mse }}|
|Second Year|{{ site.data.council.reps.second_year.mse }}|
|Third Year|{{ site.data.council.reps.third_year.mse }}|
|PEY|{{ site.data.council.reps.pey.mse }}|
|Fourth Year|{{ site.data.council.reps.fourth_year.mse }}|

|**Mechanical**||
{% for rep in site.data.council.reps.first_year.mechanical %}|First Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.second_year.mechanical %}|Second Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.third_year.mechanical %}|Third Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.pey.mechanical %}|PEY|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.fourth_year.mechanical %}|Fourth Year|{{ rep }}|
{% endfor %}

|**Mineral**||
|First Year|{{ site.data.council.reps.first_year.mineral }}|
|Second Year|{{ site.data.council.reps.second_year.mineral }}|
|Third Year|{{ site.data.council.reps.third_year.mineral }}|
|PEY|{{ site.data.council.reps.pey.mineral }}|
|Fourth Year|{{ site.data.council.reps.fourth_year.mineral }}|

|**Track One**||
|First Year|{{ site.data.council.reps.first_year.trackone }}|