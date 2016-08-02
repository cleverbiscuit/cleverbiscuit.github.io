---
layout: page
title: Get in Touch
permalink: /contact/
---

<p>We'd love to hear from you. Send us a message below if you'd like to discuss something or have a question about one of our products. We love to hear from our users!</p>

<form action="//formspree.io/mitchrenton@gmail.com" method="post" id="contact-form" class="form">

	<div class="grid">

		<div class="grid__col u-6-md">

			<div class="form__field">
				<label for="Name" class="form__label">Name <span class="form__not-requried text--muted">optional</span></label>
				<input type="text" class="form__control" name="Name" id="Name">
			</div>

		</div><!--

		--><div class="grid__col u-6-md">

			<div class="form__field">
				<label for="Email" class="form__label">Email address <span class="form__not-requried text--muted">optional</span></label>
				<input type="email" name="Email" id="Email" class="form__control">
				<p class="form__helper text--muted">If you'd like us to respond, we're going to need this. We won't ever spam you. Promise.</p>
			</div>

		</div>

	</div>

	<div class="form__field">
		<label for="Message" class="form__label">Message</label>
		<textarea name="Message" id="Message" rows="5" class="form__control" required></textarea>
	</div>

	<!-- congig -->
	<input type="hidden" name="_subject" value="cleverbiscuit.com form submission">
	<input type="text" name="_gotcha" style="display:none">
	<!-- /config -->

	<div class="text--right">

		<div class="form__field">
			<input type="submit" class="btn btn--cta form__submit" value="Send Message">
		</div>

	</div>

</form>