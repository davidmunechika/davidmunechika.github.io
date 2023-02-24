---
layout: cv
title: CV
permalink: cv/
jsarr:
- js/scripts.js
---

<h1 id="cv-title"><a href="{{ site.url }}">David Munechika</a></h1>

<p id="cv-subtitle"><i>Stamps President's Scholar at Georgia Tech</i></p>

<div>
I'm a bachelor’s candidate in <b>Computer Science</b> and Stamps President's Scholar at the Georgia Institute of Technology with degree concentrations in <b>Artificial Intelligence</b> and <b>Information Internetworks</b>.
</div>

<div class="cv-spacer"></div>

<div>
I have strong proficiencies in both object-oriented and functional programming languages including <b>Java, JavaScript, Typescript, Python, and Elixir</b>. I have experience building web and mobile applications as a full-stack developer in an agile environment, using various <b>web frameworks</b> (React, Node, Express, Phoenix), <b>database management systems</b> (PostgreSQL, MySQL, MongoDB, Firebase), <b>cloud computing services</b> (AWS, GCP), and <b>container management systems</b> (Docker, Kubernetes). My past research experience involves <b>deep learning</b> for computer vision applications, geospatial <b>data science and visualization</b>, and <b>natural language processing</b>.
</div>

<div class="cv-spacer"></div>

<div>
I have collaborated with designers, developers, engineers, and scientists while working at Apple, Amazon, Cypress, and Stord.
</div>

<!-- <div class="cv-spacer"></div>

<div>
My research is supported by a NASA Space Technology Research Fellowship.
</div> -->

<div class="cv-spacer"></div>

<div class="cv-image-links-wrapper">
	<div class="cv-image-links">
		{% for link in site.data.social-links %}
			{% if link.cv-group == 1 %}
				{% include social-link.html link=link %}
			{% endif %}
		{% endfor %}
	</div>
	<div class="cv-image-links">
		{% for link in site.data.social-links %}
			{% if link.cv-group == 2 %}
				{% include social-link.html link=link %}
			{% endif %}
		{% endfor %}
	</div>
</div>

***

## Education

{::nomarkdown}
{% for degree in site.data.education %}
{% include cv/degree.html degree=degree %}
{% endfor %}
{:/}

## Industry Experience

{% for experience in site.data.experiences %}
{% if experience.type == 'industry' %}
{% include cv/experience.html experience=experience %}
{% endif %}
{% endfor %}

## Research Experience

{% for experience in site.data.experiences %}
{% if experience.type == 'academic' %}
{% include cv/experience.html experience=experience %}
{% endif %}
{% endfor %}

## Honors and Awards

{% for award in site.data.awards %}
{% include cv/award.html award=award %}
{% endfor %}

## Publications

{% assign selectedBoolForBibtex = false %}

### Conference

{% assign conference = site.categories.papers | where: 'type', "conference" %}
{% for pub in conference %}
{% include cv/publication.html pub=pub selectedBoolForBibtex=selectedBoolForBibtex %}
{% endfor %}

## Technology Skills

{% for skill in site.data.skills %}
{% include cv/skill.html skill=skill %}
{% endfor %}

## Service

<div class="cv-service-title"><b>Reviewer</b></div>
{% for venue in site.data.reviewer %}
{% include cv/venue.html venue=venue %}
{% endfor %}

<div class="cv-service-title"><b>Member</b></div>
{% for member in site.data.memberships %}
{% include cv/member.html member=member %}
{% endfor %}

## Projects

{% for design in site.data.projects %}
{% include cv/design.html design=design %}
{% endfor %}

## References

{% for reference in site.data.references %}
{% include cv/reference.html reference=reference %}
{% endfor %}


[cv]: {{ site.url }}/cv.pdf "My CV."

[poloclub]: http://poloclub.gatech.edu "Polo Club of Data Science"
[gt]: http://gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "GT Computational Science and Engineering"
[coc]: http://www.cc.gatech.edu "GT College of Computing"

[david]: http://davidmunechika.com "David Munechika"
[polo]: http://www.cc.gatech.edu/~dchau/ "Polo Chau"

[twitter]: https:/www.twitter.com/davidmunechika "@davidmunechika"
[github]: https:/www.github.com/davidmunechika "github.com/davidmunechika"
