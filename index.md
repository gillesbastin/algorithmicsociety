---

layout:     default
title:      Bienvenue
type:       page
navigation: false
details:    true

date:       2019-10-14
image:      header-1.jpg
excerpt:    "La chaire Société algorithmique est une des chaires de recherche de l'institut <b>MIAI</b> (Multidisciplinary Institute in Artificial Intelligence) de l'Université Grenoble Alpes | The Algorithmic society chair is one of the research chairs of the University Grenoble Alpes MIAI ((Multidisciplinary Institute in Artificial Intelligence)"
gradient:   2

---

La chaire Société algorithmique conduit des recherches sur le tournant algorithmique de la société contemporaine. Elle ambitionne de relever un triple défi pour aider à comprendre ce tournant : un défi empirique consistant à étudier l'intelligence artificielle dans les contextes sociaux de son utilisation, un défi expérimental consistant à proposer une recherche multidisciplinaire innovante sur les biais de l'intelligence artificelle et un défi culturel en favorisant le développement d'une culture algorithmique parmi les étudiants en sciences sociales.|The Algorithmic society chair carries on research on the algorithmic turn of contemporary society. The chair ambitions to take a triple challenge to understand this turn : an empirical challenge by studying artificial intelligence in its immediate social settings, an experimental challenge by proposing innovative cross-disciplinary research on biases in artificial intelligence and a cultural challenge by fostering a new algorithmic literacy among social science students.

<hr>

<h2>Actualité | News</h2>
<p>Voir la rubrique « Archive » pour retrouver l'ensemble des actualités postées sur ce site. | All news are available in the "Archive" section of the site.</p>

<ul class="post-list">
{% for post in site.posts limit:site.pagination %}
      <span class="post-meta">{{ post.date | date: "%d %b %Y" }}
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
{% endfor %}
</ul>
