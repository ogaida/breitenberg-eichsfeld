---
title: hier kannst Du die Angaben zu Deinem Verein eintragen
sub_title: Alles freiwillig!
layout: post
---

Lasse die Felder unbearbeitet, wo Du keine Daten vorliegen hast oder Du nichts veröffentlichen lassen möchtest. 


<form method="post" action="./cgi-bin/vereins-input.pl">
	<div class="row gtr-50 gtr-uniform">


		{% for info in site.data.verein %}
			<div class="col-6 col-12-mobilep">
				<a style="width:400px;text-align:start;" href="javascript:void(0)" class="button">{{ info.label }} :</a>
			</div>
			<div class="col-6 col-12-mobilep">
				<input type="text" name="{{ info.key }}" id="{{ info.key }}" value="" placeholder="{{ info.placeholder }}" />
			</div>
		{% endfor %}
		<div class="col-12">
			<ul class="actions special">
				<li><input type="submit" value="Vereinsdaten aktualisieren!" /></li>
			</ul>
		</div>
	</div>
</form>
