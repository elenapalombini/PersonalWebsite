---
layout: page
title: portfolio
permalink: /portfolio/
---
{% assign projects = site.portfolio | sort: 'date' | reverse %}

{% for project in projects %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail" style="background-image:url({{ project.img }})">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <!--
        <img class="thumbnail" src="{{ project.img }}"/>
        -->
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.date | date: "%Y" }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail" style="background-image:url({{ project.img }})">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
         <!--
        <img class="thumbnail" src="{{ project.img }}"/>
        -->
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.date | date: "%Y" }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %}
