---
    layout: main
    title: My site
---

<h1>{{ page.title }}</h1>
<p>Hello World!</p>

<ol>
    {% for item in site.data.list %}
        <li>{{ item.name }} - {{ item.value }}</li>
    {% endfor %}
</ol>

<section id="posts">
    <h2>Posts</h2>
    {% for post in site.posts %}
        <a href="{{post.url}}">{{ post.title }}</a>
    {% endfor %}
</section>