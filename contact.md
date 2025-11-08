---
layout: default
title: kontaktieren Sie uns ...
subtitle: Bitte teilen Sie uns ihr Anliegen mit
toc_name: Kontakt
---

<form method="post" action="./cgi-bin/contact-request-inaktiv.pl">
	<div class="row gtr-50 gtr-uniform">
		<div class="col-6 col-12-mobilep">
			<input type="text" name="name" id="name" value="" placeholder="Name" />
		</div>
		<div class="col-6 col-12-mobilep">
			<input type="email" name="email" id="email" value="" placeholder="Ihre eigene Email-Adresse für die Validierung" />
		</div>
		<div class="col-12">
			<input type="text" name="betreff" id="subject" value="" placeholder="Betreff" />
		</div>
		<div class="col-12">
			<textarea name="text" id="message" placeholder="Ihre Nachricht an den Ortsrat ..." rows="6"></textarea>
		</div>
		<div class="col-12">
			<ul class="actions special">
				<li><input type="submit" value="Nachricht zum Ortsrat senden!" /></li>
			</ul>
		</div>
	</div>
</form>
