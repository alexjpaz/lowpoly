---
layout: post
---

{{ content }}

{% for file in page.files %}
<strong>
<a href='{{ file | relative_url }}'>Download blend file<a>
</strong>
{% endfor %}

{% for image in page.images %}
<img src='{{ image | relative_url }}' />
{% endfor %}

{% for model in page.models %}
{% include babylon-viewer.html model=model %}
{% endfor %}

