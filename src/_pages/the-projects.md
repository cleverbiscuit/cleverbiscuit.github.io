---
layout: default
title: The projects
permalink: /the-projects/
---

<div class="container">

  <div class="section">

    <h2>The Projects</h2>
      
    <div class="grid">

      {% assign projects = site.projects | sort: 'sort' %}

      {% for project in projects %}<div class="grid__col u-6-sm u-4-md u-3-lg">
        
        <div class="card card--overlay">

          <a href="{{ project.url }}">
          
            <div class="card__image">
              
              <img src="{{ site.baseurl }}/assets/images/{{ project.img }}" alt="{{ project.title }} logo">

              <div class="card__overlay"></div>

            </div>

            <div class="card__details">
              
              <h3>{{ project.title }}</h3>

            </div>

          </a>

        </div>

      </div>{% endfor %}

    </div>

  </div>

</div>