---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<style>
.entry {
    margin-bottom: 1rem;
}

.links {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: stretch;
}

.heading {
    font-size: 28px;
}

div.link {
    font-size: 20px;
    margin: 0.3rem;
    width: 100%;
}

span.link {
    padding: 0.3rem;
    background-color: #ddf;
}
</style>

{% for entry in site.data.records.entries %}
<div class="entry">
    <span class="heading">{{ entry.title }}</span>
    <div class="links">
    {% for link in entry.links %}
        <a href="{{ link.url }}">
            <div class="link">
                <span class="link">{{ link.title }}</span>
            </div>
        </a>
    {% endfor %}
    </div>
</div>
{% endfor %}
