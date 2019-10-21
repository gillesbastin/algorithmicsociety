---

layout:     default
title:      Bienvenue
type:       page
navigation: true

date:       2019-10-14
image:      header-1.jpg
excerpt:    "La chaire Société algorithmique est une des chaires de recherche de l'institut <b>MIAI</b> (Multidisciplinary Institute in Artificial Intelligence) de l'Université Grenoble Alpes. Elle conduit et soutient des recherches sur le tournant algorithmique de la société contemporaine."
gradient:   2

---

La société connaît un tournant algorithmique sans précédent. La chaire Société algorithmique va relever un triple défi pour aider à comprendre ce tournant : un défi empirique consistant à étudier l'intelligence artificielle dans les contextes sociaux de son utilisation, un défi expérimental consistant à proposer une recherche transdisciplinaire innovante sur les biais de l'intelligence artificelle et un défi culturel en favorisant le développement d'une culture algorithmique parmi les étudiants en sciences sociales.

<i>Society is experiencing an unprecedented algorithmic turn. The Algorithmic Society Chair will take a triple challenge to understand this turn : an empirical challenge by studying artificial intelligence in its immediate social settings, an experimental challenge by proposing innovative cross-disciplinary research on biases in artificial intelligence and a cultural challenge by fostering a new algorithmic literacy among social science students.</i>
<br>

---

<h2>Actualité de la chaire</h2>
<p>Voir la rubrique « Archives » pour retrouver l'ensemble des actualités postées sur ce site.</p>

<ul class="post-list">
    {% for post in site.posts limit:site.pagination %}
      <span class="post-meta">{{ post.date | date: "%d %b %Y" }}
        {{post.excerpt.length}}
      </span>
      <h3>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
          {{ post.title }}
        </a>
      </h3>
      <p class="post-excerpt">
        {{ post.excerpt }}
      </p>
      <br>
    {% endfor %}
  </ul>
