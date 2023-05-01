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
		I am a Computer Science and Biomedical Engineering undergrad at Georgia Tech. I am advised by <a href="http://www.cc.gatech.edu/~dchau/">Polo Chau</a>, who is the PI of <a href="https://poloclub.github.io">Polo Club of Data Science</a>.
	</div>
	<div style="height: 1rem"></div>
	<div class="intro-left">
		My interests encompass the intersection of <b>machine learning and human-computing interaction</b> and <b>deep learning</b>. I enjoy working on projects that utilize deep learning architectures or aim to interpret and understand how machine learning models learn.
	</div>
	<div style="height: 1rem"></div>
	<div class="intro-left">
		I am a head teaching assistant for Georgia Tech's undergraduate and graduate Machine Learning course (<a href="https://mahdi-roozbahani.github.io/CS46417641-spring2022/">CS4641 & CS7641</a>) where I was Georgia Tech's Undergraduate Teaching Assistant of the Year for 2022. If you're in my section and reading this, please feel free to reach out for anything &#8211; I won't bite.
	</div>
	<div style="height: 1rem"></div>
	<div class="intro-left">
		I have worked at Amazon Web Services (AWS) as a Software Developer Engineer intern and Qualcomm's Autonomous Driving project as a Data Engineer intern. 
	</div>
	<div style="height: 1rem"></div>
	<div class="intro-left">
		I will be pursuing my Ph.D. in Machine Learning at Carnegie Mellon University's School of Computer Science in Fall 2023! 
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
