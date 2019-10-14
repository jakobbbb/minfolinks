---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<style>
span {
    line-height: 1.8;
}
.heading {
    font-size: 28px;
}
.link {
    font-size: 20px;
    background-color: #ddf;
    padding: 0.3rem;
}
</style>

{% for entry in site.data.records.entries %}
<div class="entry">
    <span class="heading">{{ entry.title }}</span>
    <p>
    {% for link in entry.links %}
        <a class="link" href="{{ link.url }}">{{ link.title }}</a>
    {% endfor %}
    </p>
</div>
{% endfor %}
