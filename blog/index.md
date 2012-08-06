---
layout: fullNav
pageName: blog
title: Blog
tagline: The Blog
---

<article>
	<h1>Blog</h1>
	<section>
		<h2>Book Availability, Pre-Order</h2>
		<p>
			The Presentation Patterns book from Pearson (Addison-Wesley) is now available for <a href="http://www.amazon.com/Presentation-Patterns-Information-Alchemy-Presentations/dp/0321820800/ref=sr_1_2?s=books&ie=UTF8&qid=1326465927&sr=1-2">pre-order on Amazon.com</a>.
		</p>
	</section>
	<section>
		<h2>More Coming Soon</h2>
		<p>
			More blog entries and Presentation Pattern tips are coming as soon as the book hits bookshelves.
		</p>
	</section>

	<ul class="posts">
    {% for post in site.posts %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
    </ul>
</article>