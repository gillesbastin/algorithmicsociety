---

layout:		default
title:  		Archive
type:			  page
navigation: 	true

date:   		 2019-10-13
excerpt: 		"Don't let yourself be fooled by the <b>minimal and tidy overall appearance</b> of this theme — <i>you might be surprised what's included</i>."
gradient: 		2
image: 		   header-1.jpg

---

<div class="home-page">
    <h1 class="home-page__title">{{ page.title }}</h1>
    <ol class="home-page__post-list">
        {% for post in site.posts offset: site.pagination + 1 %}
        <li class="post">
            <span class="date">{{ post.date | date: "%b %-d, %Y" }}</span>
            <h2 class="title">
                <a class="link" href="{{ post.url }}">{{ post.title }}</a>
            </h2>
        </li>
        {% endfor %}
    </ol>
</div>
{% endraw}
