---
title: "Talks and Conferences"
layout: base5
name: conferences
years:
- 2023
- 2022
- 2021
- 2020
- 2019
- 2018
---
---
* TOC
{:toc}
{{ site.HR }}

<span id="upcoming-conferences"><br/></span>

### Upcoming Conferences
<br/>

[Calendar of interesting events shared between EICUG and ePIC Conferences and Talks Committees](https://eic-conferences.lbl.gov/home){:target="_blank"}


<span id="speaker-nomination-procedure"><br/></span>

{{ site.HR }}

---

### Speaker Nomination Procedure

* The Conferences and Talks Committee shall select suitable speakers taking into account expertise,
EIC related contributions, willingness to talk about a subject, working group conveners’ recommendations,
self-recommendations and recent EICUG presentations in a fair, transparent and unbiased manner.
* In order to do so, input from the community on suitable speakers is very welcome. Members are encouraged to nominate themselves too. 
<!-- * In order to do so, a list with upcoming conferences and EIC talks will be made public on the EICUG pages. Physics and other working group conveners input on suitable speakers is requested. Also members are encouraged to nominate speakers (including themselves). -->
* In order to fairly select speakers out of a large number of members, the addition of each person own expertise,
willingness to talk and potential regional/travel constraints will be added to the user database.
Each speaker should provide a link to their talks which will be available on the EICUG Conferences and Talks pages.

<span id="talk-guidelines"><br/></span>

---
 
### Talk Guidelines

In order to make sure that talks given on behalf of the EIC User Group present the project in the best way to a general audience, the following guidelines and links to several references have been assembled.

* Please provide a link to your slides at least 5 working days in advance of your presentation to the conference and talks committee <eicug-talks@eicug.org> and the steering committee.
* Present detector options without bias.
* Present the latest accelerator configuration which can be found at
[https://www.bnl.gov/eic/](https://www.bnl.gov/eic/){:target="_blank"}
* Use the documents at the following links for the information on the EIC:
[White Paper](https://inspirehep.net/literature/1206324){:target="_blank"}
and [Yellow Report](https://inspirehep.net/literature/1851258){:target="_blank"}
* For very important presentations, a rehearsal might be set up by either Conferences and Talks Committee, Steering Committee or upon request by the presenter.

If you want to recommend a candidate for a particular presentation, including yourself, please contact the Conference and Talks Committee at <eicug-talks@eicug.org>.

<!-- span id="upcoming-conferences"><br/></span -->

<!-- {{ site.HR }} -->

<!-- ### Upcoming Conferences -->
<!-- <br/ -->

<!-- {% include conf_table.md status='upcoming' %} -->

<span id="past-conferences"><br/></span>

{{ site.HR }}

### Past Conferences


{% for year in page.years %}

---

#### {{ year }}
{% include conf_table.md status='past' year=year %}
{% endfor %}
