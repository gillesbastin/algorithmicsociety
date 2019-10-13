---

layout:			default
title:  		Archive
type:			page
navigation: 	true

date:   		2019-10-13
excerpt: 		Don't let yourself be fooled by the <b>minimal and tidy overall appearance</b> of this theme — <i>you might be surprised what's included</i>.
gradient: 		2
image: 			header-2.jpg

---

<section id="archive" class="container mt-3">
      <ul class="list-group list-group-flush px-xs-1 px-md-5 mb-3">
        {% for post in paginator.posts %}
        <li class="list-group-item">
          <span class="text-muted">{{ post.date | date: "%b %d, %Y " }}</span> :
          <a href="{{ post.url }}">{{ post.title }}</a>
        </li>
        {% endfor %}
      </ul>
    </div>
</section>
