---
layout: page
title: Research
permalink: /projects/
order: 1
description: A brief overview of my research. Feel free to click on the thumbnails below and read more about them!
---

{% for project in site.projects %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
	    <br/>
	    <p>Thumbnail credit : {{ project.imgcite }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
            <br/>
	    {% if project.imgcite %}
            <p style="font-size:smaller;">Thumbnail credit : {{ project.imgcite }}</p>
	    {% endif %}
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %}
