---
layout: page
title: About
permalink: /about/
weight: 3
---

# **About Me**

Hi I am **{{ site.author.name }}** :wave:<br>
Software engineer with 3+ years of experience building scalable systems. I translate deep technical expertise into user-centered solutions by owning the product lifecycle from ideation to launch. I am driven to create tangible business value, shaping roadmaps and delivering impactful products that users love.

# **Skills**
<div class="row">
    <div class="col-lg shadow p-3 mb-5 mx-2 rounded">
        <h5 class="text-center">Product Design</h5>
            {% for skill in site.data.other-skills %}
                <div class="badge badge-pill badge-{{skill.color}} px-2 py-2"><b class="lead">{{ skill.name }}</b></div>
            {% endfor %}
    </div>
    
    <div class="col-lg shadow p-3 mb-5 mx-2 rounded">
            <h5 class="text-center">Software Engineering</h5>
        {% for skill in site.data.programming-skills %}
            <div class="badge badge-pill badge-{{skill.color}} px-2 py-2"><b class="lead">{{ skill.name }}</b></div>
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