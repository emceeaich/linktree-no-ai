---
layout: page
---
<ul
{% if site.style %}
class="{{ site.style }}"
{% endif %}
>
{% for link in site.links %}
    <li>
        <a class="{{ link[0] }}" href="{{ link[1] }}">{{ link[0] | capitalize | escape }}</a>
    </li>
{% endfor %}
</ul>

{% if site.email %}
<ul>
    <li>
        <a class="email" href="emailto:{{ site.email }}">{{ site.email }}</a>
    </li>
</ul>
{% endif %}