---
layout: page
title: coding
permalink: /coding/
---
<a href="https://github.com/iansedano">github</a>  
<a href="https://stackoverflow.com/users/10445017/ian-currie">stack overflow</a>  
<a href="https://www.codingame.com/profile/c28c694fef86992e3f41187878db77151354773">codingame</a> 

 
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
