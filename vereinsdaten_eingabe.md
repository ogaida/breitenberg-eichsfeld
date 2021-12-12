---
title: hier kannst Du die Angaben zu Deinem Verein eintragen ...
sub_title: Bitte füllen das folgende Formular aus, mit den Daten die Du angeben möchtest
layout: post
---

Alle Angaben sind freiwillig. Lasse die Felder unbearbeitet, wo keine Daten vorliegen oder Du nichts veröffentlichen möchtest. 


<form method="post" action="./cgi-bin/contact-request.pl">
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
