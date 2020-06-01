---
layout: page
title: coding
permalink: /coding/
---
<a href="https://github.com/iansedano">github</a>  
<a href="https://stackoverflow.com/users/10445017/ian-currie">stack overflow</a> 

 
<div class="flexContainer">
{% for project in site.coding %}



    <div style="background-image:url({{ project.img }})" class="box">
        
        {% if project.redirect %}
        <a href="{{ project.redirect }}" target="_blank">
        {% else %}
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% endif %}

    

        <div class="boxOverlay">
            <br>
            <h1 class="boxHeader">{{ project.title }}</h1>
        
            <p class="boxText">{{ project.description }}</p>
        </div>

        </a>
    </div>



{% endfor %}
</div>