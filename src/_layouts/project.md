---
layout: default
---

<div class="container">

    <div class="section">

        <div class="grid">

            <div class="grid__col u-6-md">
                
                <h1 class="project__title">{{ page.title }}</h1>

            </div><!--

            --><div class="grid__col u-6-md">

                <div class="project__description">

                    {{ content }}

                </div>
            
            </div>

        </div>

    </div>

    <div class="section">

        <div class="grid">
            
            {% for image in page.images %}<div class="grid__col {{ image.container }}">
                
                <img src="{{ image.image_path }}" alt="{{ image.title }}" data-zoom-padding="20" data-zoom-url="{{ image.image_path }}" data-zoom-overlay="true" class="gallery__item">

            </div>{% endfor %}

        </div>

    </div>

</div>

<div class="project__nav">

    <nav class="container">

        <ul class="nav--paged grid">
            {% if page.next-project %}
            <li class="grid__col u-6 nav__item">
                Previous Project
                <a href="{{ site.baseurl }}/projects{{ page.next-project }}">{{ page.next-project-title }}</a>
            </li>{% endif %}{% if page.prev-project %}<li class="grid__col u-6 nav__item text--right">
                Next Project
                <a href="{{ site.baseurl }}/projects{{ page.prev-project }}">{{ page.prev-project-title }}</a>
            </li>
            {% endif %}
        </ul>

    </nav>

</div>