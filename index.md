---
layout: post
title: Breitenberger Termine
---


<section id="main" class="container">

<section class="box special">
    <header class="major">
    </header>
    <!--<span class="image featured"><img src="images/pic01.jpg" alt="" /></span>-->
</section>


<!-- awesome font icons look at https://github.com/FortAwesome/Font-Awesome/tree/master/svgs/solid -->

{% for item in site.data.termine.termine %}

<div class="row">
<section class="box special features">
    <div class="features-row">
        <section>
            <span class="icon solid major fa-bell accent2"></span>
            <h3>{{ item.date }}</h3>
            <h4>{{ item.time }}</h4>
            <h4>{{ Date._parse(item.time)[:mon] }}</h4>
        </section>
        <section>
            <span class="icon solid major fa-list accent3"></span>
            <h3>{{ item.title }}</h3>
            {{ item.fleyer | markdownify }}
        </section>
    </div>
    <div class="features-row">
        <section>
            <span class="icon solid major fa-camera accent4"></span>
            <h3>{{ item.location }}</h3>
        </section>
        <section>
            <span class="icon solid major fa-info accent5"></span>
            <h3>{{ item.text | markdownify }}</h3>
        </section>
    </div>
</section>
</div>

<hr>
<hr>

{% endfor %}

</section>
