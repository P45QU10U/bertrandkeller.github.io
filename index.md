---
layout: default
title: Pensées d'un écrivain numérique de sites statiques à Rouen
image: "/assets/bertrandkeller.png"
type: website
--- 

<div class="exergue">
  <div class="wrapper">
    Vous pouvez me payer en Agnel
    <small>La monnaie locale de Rouen</small>
    Embauchez moi, pour de la <a href="/conseil-prestation-formation/">Prestation</a> ou de la <a href="/formation-jekyll-hugo/">Formation</a> !
  </div>
</div>

<div class="wrapper">
  {% assign post = site.posts.first %}
  <section class="post">
    <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
    <p class="post-meta">{{ post.date | date: "%d/%m/%Y" }}</p>
    {% if post.description %}
      <p><strong>{{ post.description }}</strong></p>
    {% endif %}
    {% if post.image %}
    {% if site.environment != 'development' %}
    {% cloudinary {{post.image}} alt="{{post.title}}" %}
    {% else %}
    <img src="{{ post.image }}" alt="{{ post.title }}">
    {% endif %}
    {% endif %}
    {{ post.content | markdownify }}
  </section>

  <div class="pagination--prevnext" role="navigation">
    {% if post.previous %}
    <div class="pagination--prev">
      <a class="pagination--item" href="{{ post.previous.url }}">
        {{ post.previous.title }}
      </a>
    </div> 
    {% endif %}

    {% if post.title == 'Transmutation' %} 
    <div class="pagination--prev">
      <a class="pagination--item" href="/2015/10/03/parisweb-cest-quoi-les-metiers-du-web">
        ParisWeb - c'est quoi les métiers du web ?
      </a>
    </div>
    {% endif %}

    {% if post.next %}
    <div class="pagination--next">
      <a class="pagination--item" href="{{ post.next.url }}">
        {{ post.next.title }}
      </a>
    </div>
    {% endif %}
  </div>
</div>

