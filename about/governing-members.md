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
|**Chemical**| |
|First Year|{{ site.data.council.reps.chemical.first_year }}|
|Second Year|{{ site.data.council.reps.chemical.second_year }}|
|Third Year|{{ site.data.council.reps.chemical.third_year }}|
|PEY|{{ site.data.council.reps.chemical.pey }}|
|Fourth Year|{{ site.data.council.reps.chemical.fourth_year }}|

|**Civil**| |
|First Year|{{ site.data.council.reps.civil.first_year }}|
|Second Year|{{ site.data.council.reps.civil.second_year }}|
|Third Year|{{ site.data.council.reps.civil.third_year }}|
{% for rep in site.data.council.reps.civil.pey %}|PEY|{{ rep }}|
{% endfor %}|Fourth Year|{{ site.data.council.reps.civil.fourth_year }}|

|**ECE**| |
{% for rep in site.data.council.reps.ece.first_year %}|First Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.ece.second_year %}|Second Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.ece.third_year %}|Third Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.ece.pey %}|PEY|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.ece.fourth_year %}|Fourth Year|{{ rep }}|
{% endfor %}

|**EngSci**| |
{% for rep in site.data.council.reps.engsci.first_year %}|First Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.engsci.second_year %}|Second Year|{{ rep }}|
{% endfor %}|Third Year|{{ site.data.council.reps.engsci.third_year }}|
|PEY|{{ site.data.council.reps.engsci.pey }}|
|Fourth Year|{{ site.data.council.reps.engsci.fourth_year }}|

|**Industrial**| |
{% for rep in site.data.council.reps.industrial.first_year %}|First Year|{{ rep }}|
{% endfor %}|Second Year|{{ site.data.council.reps.industrial.second_year }}|
|Third Year|{{ site.data.council.reps.industrial.third_year }}|
|PEY|{{ site.data.council.reps.industrial.pey }}|
|Fourth Year|{{ site.data.council.reps.industrial.fourth_year }}|

|**MSE**| |
|First Year|{{ site.data.council.reps.mse.first_year }}|
|Second Year|{{ site.data.council.reps.mse.second_year }}|
|Third Year|{{ site.data.council.reps.mse.third_year }}|
|PEY|{{ site.data.council.reps.mse.pey }}|
|Fourth Year|{{ site.data.council.reps.mse.fourth_year }}|

|**Mechanical**| |
{% for rep in site.data.council.reps.mechanical.first_year %}|First Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.mechanical.second_year %}|Second Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.mechanical.third_year %}|Third Year|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.mechanical.pey %}|PEY|{{ rep }}|
{% endfor %}{% for rep in site.data.council.reps.mechanical.fourth_year %}|Fourth Year|{{ rep }}|
{% endfor %}

|**Mineral**| |
|First Year|{{ site.data.council.reps.mineral.first_year }}|
|Second Year|{{ site.data.council.reps.mineral.second_year }}|
|Third Year|{{ site.data.council.reps.mineral.third_year }}|
|PEY|{{ site.data.council.reps.mineral.pey }}|
|Fourth Year|{{ site.data.council.reps.mineral.fourth_year }}|

|**Track One**| |
|First Year|{{ site.data.council.reps.trackone.first_year }}|
