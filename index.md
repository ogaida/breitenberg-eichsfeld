---
layout: post
title: Breitenberger Termine
---


<section>

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

