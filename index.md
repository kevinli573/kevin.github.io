---
layout: home
title: Home
---

<div id ="intro-wrapper" class="l-middle">
	<div id="intro-title-wrapper" class="intro-left">
		<h1 id="intro-title">Hi, I'm Kevin Li</h1>
	</div>
	<div class="intro-left">
	<div class="intro-left">
		I am a second year Ph.D. student at CMU's Machine Learning Department, where I am fortunate enough to be co-advised by both <a href="https://twitter.com/_albertgu">Prof. Albert Gu</a> and <a href="https://zicokolter.com">Prof. Zico Kolter</a>. Previously, I was a Computer Science and Biomedical Engineering undergrad at Georgia Tech, where I had a wonderful time advised by <a href="http://www.cc.gatech.edu/~dchau/">Prof. Polo Chau</a>.
	</div>
	<div style="height: 1rem"></div>
	<div class="intro-left">
		I am interested in developing efficient deep learning architectures and methods and scaling inference compute for reasoning and general performance. Please reach out if you are interested in collaborating!
	</div>
	<div style="height: 1rem"></div>
	<div class="intro-left">
		I have had stints at Amazon Web Services (AWS), Qualcomm, and Bosch in both engineering and research-focused roles. 
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
		<!-- <div id="intro-cv"><a href="/cv">Here's my CV.</a></div> -->
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

<hr class="l-middle home-hr">

<h2 class="feature-title l-middle">
	<a href="/cv#honors-and-awards">Honors and Awards</a>
</h2>
{% for award in site.data.awards %}
{% include cv/award.html award=award %}
{% endfor %}

<hr class="l-middle home-hr">

<h2 class="feature-title l-middle">
	<a href="/cv#academic-research-experience">Research Experience</a>
</h2>
{% for experience in site.data.experiences %}
{% if experience.type == 'academic' %}
{% include cv/experience.html experience=experience %}
{% endif %}
{% endfor %}

[gt]: http://www.gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "Georgia Tech Computational Science and Engineering"
[coc]: http://www.cc.gatech.edu "Georgia Tech College of Computing"

[cv]: {{ site.url }}/cv
[polo]: http://www.cc.gatech.edu/~dchau/ "Polo Chau"
