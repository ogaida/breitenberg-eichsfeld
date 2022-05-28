---
layout: default
title: Breitenberg im Eichsfeld
---

<section id="main" class="container">

<section class="box special">
<header class="major">
<h3>Der neue Ortsrat 2021
<br />
Bürgermeisterin: Katja Neumann
<br />
Stellverter: Gregor Wippermann
</h3>
<p> weitere Mitglieder unseres Ortsrates sind: <br>
Dieter Eckermann, Dominik Deppe, Matthias Nolte, <br>
Martin Winkler und Andrew Gieseler</p>
</header>
<span class="image featured"><img src="images/banner.jpg" alt="" /></span>
</section>


</section>

<section id="cta">

<h2>Termine</h2>
        {% for item in site.data.termine.termine %}
          <div class="resume-item d-flex flex-column flex-md-row justify-content-between mb-5">
            <div class="resume-content">
              <h3 class="mb-0">{{ item.title }}</h3>
              <p>{{ item.text | markdownify }}</p>
            </div>
          </div>
        {% endfor %}

</section>

