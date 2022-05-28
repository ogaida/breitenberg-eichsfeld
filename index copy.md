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

<section>

<h2>Termine</h2>
        <table border=0>
        {% for item in site.data.termine.termine %}
            <tr>
                <td>
                    <table border=0>
                        <tr>
                            <td>
                            {{ item.title }}
                            </td>
                        </tr>
                        <tr>
                            <td>
                            {{ item.date }}
                            </td>
                        </tr>
                        <tr>
                            <td>
                            {{ item.wo }}
                            </td>
                        </tr>
                    </table>
                </td>
                <td>
                    {{ item.text | markdownify }}
                </td>
            </tr>
        {% endfor %}
        </table>    
</section>

