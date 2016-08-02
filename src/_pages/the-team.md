---
layout: default
title: Who are we?
permalink: /the-team/
---

<div class="container">

	<div class="section">

		<h1>The Team</h1>
		
		<div class="grid">

		{% for member in site.data.members %}<div class="grid__col u-6-sm u-4-md">

				<div class="card">

					<div class="card__image card__image--profile">

						<img src="{{ site.baseurl }}/assets/images/{{ member.img }}.png" alt="{{ member.name }} hand drawn {{ site.title }} character">

					</div>

					<div class="card__details">

						<h2 class="card__title">{{ member.name }}</h2>

						<p>{{ member.bio }}</p>

					</div>

					{% if member.public %}

					<div class="card__links">

						<ul class="list--inline list--inline--delimited list--stripped text--center">
							<li><a class="card__link" href="https://twitter.com/{{ member.twitter }}" title="Visit {{ member.name }} on Twitter"><img src="{{ site.baseurl }}/assets/images/twitter.svg" alt="Twitter icon"> Twitter</a>
							{% if member.github %}
						    <li><a class="card__link" href="https://github.com/{{ member.github }}" title="Visit {{ member.name }} on GitHub"><img src="{{ site.baseurl }}/assets/images/github.svg" alt="GitHub icon"> Github</a>
						    {% endif %}
						    <li><a class="card__link" href="{{ member.website }}" title="Visit {{ member.name }}'s website"><img src="{{ site.baseurl }}/assets/images/earth.svg" alt="Website icon"> Website</a>
						</ul>

					</div>

					{% endif %}

				</div>

			</div>{% endfor %}

		</div>

	</div>

</div>