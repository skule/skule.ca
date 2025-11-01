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
|**First Year**||
|Chemical|{{ site.data.council.reps.first_year.chemical }}|
|Civil|{{ site.data.council.reps.first_year.civil }}|
{% for rep in site.data.council.reps.first_year.ece %}|ECE|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.first_year.engsci %}|EngSci|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.first_year.industrial %}|Industrial|{{ rep }}|
{% endfor %}|MSE|{{ site.data.council.reps.first_year.mse }}|
{% for rep in site.data.council.reps.first_year.mechanical %}|Mechanical|{{ rep }}|
{% endfor %}|Mineral|{{ site.data.council.reps.first_year.mineral }}|
|Track One|{{ site.data.council.reps.first_year.trackone }}|

|**Second Year**||
|Chemical|{{ site.data.council.reps.second_year.chemical }}|
|Civil|{{ site.data.council.reps.second_year.civil }}|
{% for rep in site.data.council.reps.second_year.ece %}|ECE|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.second_year.engsci %}|EngSci|{{ rep }}|
{% endfor %}|Industrial|{{ site.data.council.reps.second_year.industrial }}|
|MSE|{{ site.data.council.reps.second_year.mse }}|
{% for rep in site.data.council.reps.second_year.mechanical %}|Mechanical|{{ rep }}|
{% endfor %}|Mineral|{{ site.data.council.reps.second_year.mineral }}|

|**Third Year**||
|Chemical|{{ site.data.council.reps.third_year.chemical }}|
|Civil|{{ site.data.council.reps.third_year.civil }}|
{% for rep in site.data.council.reps.third_year.ece %}|ECE|{{ rep }}|
{% endfor %}|EngSci|{{ site.data.council.reps.third_year.engsci }}|
|Industrial|{{ site.data.council.reps.third_year.industrial }}|
|MSE|{{ site.data.council.reps.third_year.mse }}|
{% for rep in site.data.council.reps.third_year.mechanical %}|Mechanical|{{ rep }}|
{% endfor %}|Mineral|{{ site.data.council.reps.third_year.mineral }}|

|**PEY**||
|Chemical|{{ site.data.council.reps.pey.chemical }}|
{% for rep in site.data.council.reps.pey.civil %}|Civil|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.pey.ece %}|ECE|{{ rep }}|
{% endfor %}|EngSci|{{ site.data.council.reps.pey.engsci }}|
|Industrial|{{ site.data.council.reps.pey.industrial }}|
|MSE|{{ site.data.council.reps.pey.mse }}|
{% for rep in site.data.council.reps.pey.mechanical %}|Mechanical|{{ rep }}|
{% endfor %}|Mineral|{{ site.data.council.reps.pey.mineral }}|

|**Fourth Year**||
|Chemical|{{ site.data.council.reps.fourth_year.chemical }}|
|Civil|{{ site.data.council.reps.fourth_year.civil }}|
{% for rep in site.data.council.reps.fourth_year.ece %}|ECE|{{ rep }}|
{% endfor %}|EngSci|{{ site.data.council.reps.fourth_year.engsci }}|
|Industrial|{{ site.data.council.reps.fourth_year.industrial }}|
|MSE|{{ site.data.council.reps.fourth_year.mse }}|
{% for rep in site.data.council.reps.fourth_year.mechanical %}|Mechanical|{{ rep }}|
{% endfor %}|Mineral|{{ site.data.council.reps.fourth_year.mineral }}|
