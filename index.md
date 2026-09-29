---
    layout: main
    title: My site
---

<script src="/assets/scripts/main.js"></script>

<h1>{{ page.title }}</h1>
<p>Hello World!</p>

<ol>
    {% for item in site.data.list %}
        <li>{{ item.name }} - {{ item.value }}</li>
    {% endfor %}
</ol>

<section id="posts">
    <h2>Posts</h2>
    <a href="/blog">Blog</a>
</section>