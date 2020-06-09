---
layout: page
permalink: /music/
title: music
description: my musical projects
---
<a href="https://www.instagram.com/iansedano/?hl=en">instagram</a><br>
<a href="https://soundcloud.com/ianinthecave">soundcloud</a> <br>
<a href="https://www.youtube.com/channel/UCgJV7OHO1uVPnG89j4ksm7Q">youtube</a>
<br><br>

<ul class="post-list">
{% for post in site.music reversed %}
    <li>
        <a class="post-list-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}</p>
      </li>
{% endfor %}
</ul>