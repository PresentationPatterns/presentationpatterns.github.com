---
layout: fullNav
pageName: blog
title: Blog
tagline: The Blog
---

<article>
	<h1>Blog</h1>

	<section>
    {% for post in site.posts %}
        
        <section>
            <a href="{{ site.pathing.baseURL }}{{ BASE_PATH }}{{ post.url }}">
                <h2>{{ post.date | date_to_string }} &raquo; {{ post.title }}</h2>
            </a>
            <p>{{ post.tagline }}</p>
            <a href="{{ site.pathing.baseURL }}{{ BASE_PATH }}{{ post.url }}">
                <p>Read more...</p>
            </a>
        </section>
        
    {% endfor %}
    </section>
</article>
