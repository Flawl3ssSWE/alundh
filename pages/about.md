---
layout: page
title: About
permalink: /about/
weight: 3
---

{% assign dateStart = "2001-10-13" | date: '%s' %}
{% assign nowTimestamp = 'now' | date: '%s' %}

{% assign diffSeconds = nowTimestamp | minus: dateStart %}
{% assign diffDays = diffSeconds | divided_by: 3600 | divided_by: 24 | divided_by: 365 %}

# **About Me**

Hello, I am **{{ site.author.name }}** :wave:, a {{ diffDays | round: 0 }}-year-old engineer from Sweden :sweden:.<br>
I am passionate about technology and hiking with a sweet spot for 3D printing, home automation, mechatronics, and cyber security! 

My fascination for 3D Printers started back in 2017 with the purchase of my first 3D Printer, a Tevo Tarantula. 
A simple printer kit from China that I upgraded for far more than the original cost of the kit. In the end, I redesigned it from the ground up back in 2019/2020, so it now features two independently controllable extruders. 
Allowing for printing two of the same parts at the same time, and multicolor printing. My second 3D Printer was a Prusa 3D MK3 a printer that I still to this day use. It was great from the start, but I still decided to upgrade it with a more rigid frame and a better extruder.

My love for mechatronics came almost naturally after years of watching cool projects being built by others. I decided to join the action, by building cool projects that had been designed by others' and started to design my own. My go-to kind of project is some kind of home automation, making my life in some way easier (usually :wink:). Some of my favorites that are designed by me can be found under the "Projects" tab (coming soon).

My love for hiking began at Store Mosse National Park outside Värnamo, evolving from casual walks into explorations of some of Sweden's most incredible places. Last summer, me and a friend hiked and lived in a tent for 19 while hiking along Kungsleden, between Hemavan and Saltoloukta, a hike totaling 360 km. If you ever find yourself around Åre in the summer, I highly recommend taking a day to visit Jämtlands Pyramiderna, located in Vålådalens Nature Reserve. It is a 22 km hike, which might sound like a long trek, but seeing the pyramids with your own eyes is, in my humble opinion, well worth it!

My interest in cyber security, came sometime between 2016 and 2018, after stumbling upon the great site [haveibeenpwned.com](https://haveibeenpwned.com){:target="_blank"}{:rel="noopener noreferrer"} by Troy Hunt and finding out some of my emails had appeared in some data breaches. Since then it has flourished and I am now interested in keeping myself more secure with better passwords and physical two factor authentication keys. I also try to keep my home network safe by running pfSense with multiple segmented VLANs to minimize the attack vector. In the end, this has led me to choose to orient my future career and master's degree towards cyber security. In my spare time I use TryHackMe to learn more about cyber security.

All of my interests combined led me to decide to be a part of the board for the student association Lindholmens Makerspace during my third year at Chalmers, offering help and space for other students to build and design at Chalmers. During my time at Lindholmens Makerspace I was responsible for taking notes at our meetings, our 3D Printers, designing the posters we put up around Chalmers advertising our events, knowing what we owned and where it was located, and keeping our tools and electronics stock up to date with what the members wanted.

<style>
	.column {
		float: left;
		width: 50%;
		padding: 10px;
	}
	
	.row:after {
		content: "";
		display: table;
		clear: both;
	}
	
	ul.Software li {
		margin-bottom: 23px;
	}
	
	h1.Title-Skills {
		margin-bottom: -30px;
	}
	
	@media screen and (max-width: 600px) {
		.column {
			width: 100%;
	}
</style>

<body>

<h1 class="Title-Skills"><b>Skills</b></h1>
<div class="row">
  <div class="column">
    <h2>Programming languages</h2>
    <h5>Good knowledge of:</h5>
	<ul>
		<li>Arduino (C)</li>
		<li>Python</li>
		
	</ul>
	<h5>Some knowledge of:</h5>
	<ul>
		<li>GoLang</li>
		<li>HTML/PHP/CSS</li>
		<li>SQL</li>
		<li>VHDL</li>
		<li>C++</li>
		<li>C#</li>
		<li>Assembler</li>
	</ul>
	<h5>Have touched:</h5>
	<ul>
		<li>CircuitPython</li>
		<li>JavaScript</li>
	</ul>
  </div>
  
  <div class="column">
    <h2>Software</h2>
    	<ul class="Software">
			<li>AutoDesk Fusion 360</li>
			<li>BurpSuite</li>
			<li>MetaSploit</li>
			<li>Nmap</li>
			<li>Microsoft Office</li>
			<li>Microsoft PowerAutomate</li>
			<li>Microsoft SharePoint</li>
			<li>Adobe Photoshop</li>
			<li>Adobe Illustrator</li>
		</ul>
  </div>
</div>

<div class="row">
{% include about/timeline.html %}
</div>