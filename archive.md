---

layout:		    default
title:  		Archive
type:			page
navigation: 	true

date:   		 2019-10-13
excerpt: 		"Retrouvez sur cette page tous les articles postés sur le site."
gradient: 		2
image: 		    header-1.jpg

---

<div class="home-page">
    <ol class="home-page__post-list">
        {% for post in site.posts offset: site.pagination + 1 %}
        <li class="post">
            <span class="date">{{ post.date | date: "%b %-d, %Y" }}</span>
                <a class="link" href="{{ post.url }}">{{ post.title }}</a>
        </li>
        {% endfor %}
    </ol>
</div>
