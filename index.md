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

{% for post in paginator.posts %}

  {% include summary.html %}
  
{% endfor %}
