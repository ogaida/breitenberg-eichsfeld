---
layout: post
title: Breitenberg
---


<section id="main" class="container">

    <!--
    <section class="box special">
        <header class="major">
        </header>
        <h2>Erntedankaltar vom 1. Oktober 2022</h2>
        <p>Herzlichen Dank im Namen der Tafel Duderstadt an alle fleißigen Spender aus Breitenberg!</p>
        <span class="image featured"><img src="images/erntedank2022_2.jpg" alt="" /></span>
        <span class="image featured"><img src="images/erntedank2022.jpg" alt="" /></span>    
    </section>
    -->
    
<section class="box special">
    <h2>wichtige Termine in Breitenberg</h2>
</section>

<!-- awesome font icons look at https://github.com/FortAwesome/Font-Awesome/tree/master/svgs/solid -->




    {% assign yesterday = 'now' | date: '%s' | minus:'86400' | times: 1 %}

    {% for item in site.data.termine.termine %}

        {% assign termin_date = item.date | date: '%s' | times: 1 %}
        {% if yesterday < termin_date %}

    <div class="row">
    <section class="box special features">
        <div class="features-row">
            <section>
                <span class="icon solid major fa-bell accent2"></span>
                <h3>{{ item.date }}</h3>
                <h4>{{ item.time }}</h4>
            </section>
            <section>
                <span class="icon solid major fa-list accent3"></span>
                <h3>{{ item.title }}</h3>
                {{ item.fleyer }}
            </section>
        </div>
        <div class="features-row">
            <section>
                <span class="icon solid major fa-camera accent4"></span>
                <h3>{{ item.location }}</h3>
            </section>
            <section>
                <span class="icon solid major fa-info accent5"></span>
                <h3 style="text-align: left;margin-left: 20px">{{ item.text | markdownify }}</h3>
            </section>
        </div>
    </section>
    </div>

    <hr>
    <hr>
        {% endif %}
    {% endfor %}

</section>
