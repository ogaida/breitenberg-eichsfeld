---
layout: default
title: Breitenberg im Eichsfeld
---

<section id="main" class="container">

<section class="box special">

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
                            {{ item.location }}
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

</section>
