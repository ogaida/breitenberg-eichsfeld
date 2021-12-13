---
title: hier kannst Du die Angaben zu Deinem Verein eintragen
sub_title: Alles freiwillig!
layout: post
---

Lasse die Felder unbearbeitet, wo Du keine Daten vorliegen hast oder Du nichts veröffentlichen lassen möchtest. 


<form method="post" action="./cgi-bin/vereins-input.pl">
	<div class="row gtr-50 gtr-uniform">
		<div class="col-4 col-12-mobilep">
			<a style="width:300px;text-align:start;" href="javascript:void(0)" class="button">Verein :</a>
		</div>
		<div class="col-8 col-12-mobilep">	
			<select name="verein" id="verein">
				<option value="" disabled selected>Bitte den Verein auswählen</option>
				{% for verein in site.data.verein.vereinlist %}
					<option value="{{ verein.key }}">{{ verein.name }}</option>
				{% endfor %}
			</select>
		<div>					
		{% for info in site.data.verein.formdata %}
			<div class="col-4 col-12-mobilep">
				<a style="width:300px;text-align:start;" href="javascript:void(0)" class="button">{{ info.label }} :</a>
			</div>
			<div class="col-8 col-12-mobilep">
				<input type="text" name="{{ info.key }}" id="{{ info.key }}" value="" placeholder="{{ info.placeholder }}" />
			</div>
		{% endfor %}
		<br>
		<div class="col-12">
			<ul class="actions special">
				<li><input type="submit" value="Vereinsdaten aktualisieren!" /></li>
			</ul>
		</div>
	</div>
</form>
