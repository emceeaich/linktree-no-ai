---
layout: home
---
<ul>
{% for link in site.links %}
<li>
    <a href="{{link[1]}}">{{link[0]}}</a>
</li>
{% endfor %}
</ul>
