---
layout: home
title: Home
---

<div id ="intro-wrapper" class="l-middle">
	<div id="intro-title-wrapper" class="intro-left">
		<h1 id="intro-title">Hi, I'm David Munechika</h1>
		<div id="intro-subtitle">
			I'm a Stamps President's Scholar at Georgia Tech
		</div>
	</div>
	<div class="intro-left">
	<div class="intro-left">
		I'm a master's candidate in <b>Computer Science</b> and Stamps President's Scholar at the Georgia Institute of Technology with a degree specialization in <b>Machine Learning</b>.
	</div>
	<div style="height: 1rem"></div>
	<div class="intro-left">
	I have strong proficiencies in both object-oriented and functional programming languages including <b>Python, Java, JavaScript/Typescript, Swift, and Elixir</b>. I have experience building web and mobile applications as a full-stack developer in an agile environment, using various <b>frameworks</b> (React, Node, Express, Phoenix, SwiftUI), <b>database management systems</b> (DynamoDB, PostgreSQL, MySQL, MongoDB, Firebase), <b>cloud computing services</b> (AWS, GCP), and <b>container management systems</b> (ECS, Fargate, Docker, Kubernetes). My past research experience involves <b>interactive visualization</b> for machine learning, <b>deep learning</b> for computer vision applications, geospatial <b>data science</b>, and <b>generative AI</b>.
	</div>
	<div style="height: 1rem"></div>
	<div>
		I have collaborated with numerous designers, developers, engineers, and scientists while working at <img class="intro-logo" style="width: 28px; padding-bottom: 6px;" src="/images/apple.png"> Apple, <img class="intro-logo" style="width: 18px; padding-bottom: 2px;" src="/images/amazon.svg"> Amazon, <img class="intro-logo" style="width: 24px; padding-bottom: 5px" src="/images/cypress.png"> Cypress, and <img class="intro-logo" style="width: 20px; padding-bottom: 5px" src="/images/stord.png"> Stord.
	</div>
</div>

<div class="intro-right">
	<img id="intro-image" class="intro-right" src="/images/portrait.jpg">
	<div style="height: 0.5rem"></div>
	<div id="intro-image-links" class="intro-right">
		{% for link in site.data.social-links %}
			{% if link.on-homepage == true %}
				{% include social-link.html link=link %}
			{% endif %}
		{% endfor %}
	</div>
	<div style="height: 0.5rem"></div>
	<div id="intro-cv-wrapper" class="intro-right">
		{% for link in site.data.social-links %}
			{% if link.id == "cv-web" %}
				{% include social-link.html link=link %}
			{% endif %}
		{% endfor %}
	</div>
	</div>
</div>

<hr class="l-middle home-hr">

<h2 class="feature-title l-middle">
	Featured <a href="/cv#publications">Research Publications</a>
</h2>
<div class="cover-wrapper l-screen">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' %}
	{% for feature in sortedPublications %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>

<h2 class="feature-title l-middle">
	Past <a href="/cv#industry-experience">Internship Experience</a>
</h2>
<div class="cover-wrapper l-screen">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' %}
	{% for feature in sortedPublications %}
		{% if feature.dissertation == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>

<!-- <h2 class="feature-title l-middle">
	<a href="{{ site.url }}/everything-else" style="color: #303030">Everything Else</a>
</h2>
<div id="everything-else" class="l-middle">
	<a href="{{ site.url }}/projects"><div>Projects</div></a>
	<a href="{{ site.url }}/blog"><div>Blog</div></a>
	<a href="{{ site.url }}/stuff-i-use"><div>Stuff I Use</div></a>
	<a href="{{ site.url }}/monthly-music"><div>Monthly Music</div></a>
	<a href="{{ site.url }}/archive"><div>Archive</div></a>
</div> -->



[gt]: http://www.gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "Georgia Tech Computational Science and Engineering"
[coc]: http://www.cc.gatech.edu "Georgia Tech College of Computing"

[cv]: {{ site.url }}/cv
[polo]: http://www.cc.gatech.edu/~dchau/ "Polo Chau"
[alex]: http://va.gatech.edu/endert/ "Alex Endert"
[poloclub]: http://poloclub.gatech.edu "Polo Club of Data Science"
[nstrf]: https://www.nasa.gov/strg/nstrf "NASA Space Technology Research Fellowship"