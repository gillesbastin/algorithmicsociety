---

layout:		default
title:  		Archive
type:			page
navigation: 	true

date:   		2019-10-13
excerpt: 		Don't let yourself be fooled by the <b>minimal and tidy overall appearance</b> of this theme — <i>you might be surprised what's included</i>.
gradient: 		2
image: 		header-1.jpg

---

<ul>
 {% for post in paginator.posts %}
  <li class="list-group-item">
   <span class="text-muted">{{ post.date | date: "%b %d, %Y " }}</span> :
   <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
 {% endfor %}
</ul>
