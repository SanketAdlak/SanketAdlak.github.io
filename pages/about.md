---
layout: page
title: About
permalink: /about/
weight: 3
---

# **About Me**

Hi I am **{{ site.author.name }}** :wave:<br>
I’m a software engineer with 3+ years of experience building scalable systems. I use my technical expertise to create solutions that focus on user needs, managing the entire product process—from the first idea to the final launch. I’m passionate about creating real business value, shaping product roadmaps, and delivering products that users love.

# **Skills**
<div class="row">
    <div class="col-lg shadow p-3 mb-5 mx-2 rounded">
        <h4 class="text-center">Product Design</h4>
            {% for skill in site.data.other-skills %}
                <div class="badge badge-pill badge-{{skill.color}} p-2 m-1"><b class="lead">{{ skill.name }}</b></div>
            {% endfor %}
    </div>
    
    <div class="col-lg shadow p-3 mb-5 mx-2 rounded">
            <h4 class="text-center">Software Engineering</h4>
        {% for skill in site.data.programming-skills %}
                <div class="badge badge-pill badge-{{skill.color}} p-2 m-1"><b class="lead">{{ skill.name }}</b></div>
        {% endfor %}
    </div>
</div>
<!-- 
<div class="row">   

{% include about/skills.html title="Software Engineering" source=site.data.programming-skills %}
{% include about/skills.html title="Product Design" source=site.data.other-skills %}
</div> 
-->

# **Experience**
<div class="row">
{% include about/timeline.html %}
</div>