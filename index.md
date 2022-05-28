---
layout: post
title: Breitenberger Termine
---


<section id="main" class="container">




    {% for item in site.data.termine.termine %}

    <section class="box special features">
        <div class="features-row">
            <section>
                <span class="icon solid major fa-bolt accent2"></span>
                <h3>{{ item.date }}</h3>
            </section>
            <section>
                <span class="icon solid major fa-chart-area accent3"></span>
                <h3>{{ item.title }}</h3>
            </section>
        </div>
        <div class="features-row">
            <section>
                <span class="icon solid major fa-cloud accent4"></span>
                <h3>{{ item.location }}</h3>
            </section>
            <section>
                <span class="icon solid major fa-lock accent5"></span>
                <p>{{ item.text | markdownify }}</p>
            </section>
        </div>
    </section>
    {% endfor %}

</section>
