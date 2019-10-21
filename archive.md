---

layout:		default
title:  	Archive
type:		page
navigation: 	true

date:   	2019-10-13
excerpt: 	"Retrouvez sur cette page tous les articles postés sur le site."
gradient: 	2
image: 		header-1.jpg

---

<div class="home-page">
        {% for post in site.posts offset: site.pagination + 1 %}
        <ul class="home-page__post-list">
        <li class="post">
            <span class="date">{{ post.date | date: "%b %-d, %Y" }}</span>
                |
                <a class="link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </li>
        </ul>
        {% endfor %}
</div>
