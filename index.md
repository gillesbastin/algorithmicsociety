---

layout:     default
title:      Bienvenue
type:       home
navigation: true

date:       2019-10-14
image:      header-1.jpg
excerpt:    "La chaire Société algorithmique est une des chaires de recherche de l'institut <a href = "https://miai.univ-grenoble-alpes.fr/">MIAI</a> (Multidisciplinary Institute in Artificial Intelligence) de l'Université Grenoble Alpes. Elle conduit et soutient des recherches sur le tournant algorithmique de la société contemporaine."
gradient:   2

---

Society is experiencing an unprecedented algorithmic turn. The Algorithmic Society Chair will take a triple challenge to understand this turn : an empirical challenge by studying AI in its immediate social settings, an experimental challenge by proposing innovative cross-disciplinary research on biases in AI and a cultural challenge by fostering a new AI literacy among social science students.

<h2>Actualité de la chaire</h2>
<p>These are the last posts documenting the activity of the chair.</p>

<ul class="post-list">
    {% for post in site.posts limit:site.pagination %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}
        {{post.excerpt.length}}
      </span>
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
          {{ post.title }}
        </a>
      </h2>
      <p class="post-excerpt">
        {{ post.excerpt }}
      </p>
      <br>
    </li>
    {% endfor %}
  </ul>
