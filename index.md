---

layout:     default
title:      Présentation de la chaire
type:       home
navigation: true

date:       2019-10-14
image:      header-1.jpg
excerpt:    "Society is experiencing an unprecedented algorithmic turn. The Algorithmic Society Chair will take a triple challenge to understand this turn : an empirical challenge by studying AI in its immediate social settings, an experimental challenge by proposing innovative cross-disciplinary research on biases in AI and a cultural challenge by fostering a new AI literacy among social science students."
gradient:   1

---

<h2>Last updates</h2>
<p>These are the last posts documenting the activity of the chair.</p>

<div class="summary">
        
<h4>{{ post.date | date: '%b %-d, %Y' | prepend: '<b>' | append: '</b>' }}</h4>

{% if post.author %}
<p>By <b>{{ post.author }}</b></p>
{% endif %}

{% if post.url %}
<a href="{{ post.url }}" title="Read Post" class="icon image">{{ post.content | reading_time_as_i }}</a>
{% endif %}

{% if post.title %}
<h2><a href="{{ post.url | prepend: site.baseurl }}" title="{{ post.title }}">{{ post.title }}</a></h2>
{% endif %}
    
<p>{{ post.excerpt | remove: '<p>' | remove: '</p>' }} <a href="{{ post.url | prepend: site.baseurl }}" title="Read More" class="more">Read More</a></p>

</div>
