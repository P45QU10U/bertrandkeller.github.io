---
title: Jekyll - Un thème pour artisans
description: "Site présentant les œuvres d'artisans avec un répertoire synchronisé pour l'édition"
url: http://jekyll-for-craftman.netlify.com/
herbergement: Github
image: jekyll-for-craftman-site.png
---

## Processus éditorial

**Objectif :** éditer des contenus sans jamais avoir accès à une administration de contenu.

### Les œuvres

Pour chaque œuvre, nous avons :

1. Un titre (unique)
2. Une catégorie (unique)
3. Un nom (spécifique)
4. Un crédit (spécifique)

L'objectif est d'ajouter une image dans un répertoire et de l'associer à une page pour qu'elle s'affiche dans une liste.  
Pour les œuvres qui ont plusieurs images, il est possible de les ajouter dans la liste mais sans qu'elles s'affichent sur la page de collection générale ; elles s'afficheront dans le détail de chaque œuvre (ex: devant/derrière, dessus/dessous).

<div>
{% cloudinary /assets/casestudies/jekyll-for-craftman-images.png alt="Jekyll - Un thème pour artisans" %}
</div>

1. Une liste d'œuvres (ex: [Liste d'œuvres](http://jekyll-for-craftman.netlify.com/fr/collections/))
2. Une fiche œuvre (ex: [Fiche œuvre](http://jekyll-for-craftman.netlify.com/fr/raku/vase-rouge/))

<div>
{% cloudinary /assets/casestudies/jekyll-for-craftman-detail.png alt="Jekyll - Un thème pour artisans" %}
</div>

### Les pages

Les pages sont des fichiers Markdown spécifiques, elles s'ajoutent à l'aborescence du menu principal. Un champ de l'entête de la page (ex: slug: raku) permet d'afficher toutes les images du répertoire images (décrit ci-dessus) dont le nom commence par le slug (ex: raku-Vases+vase-rouge-bombé+principal+yasefanprod)

<div>
{% cloudinary /assets/casestudies/jekyll-for-craftman-pages.png alt="Jekyll - Un thème pour artisans" %}
</div>

Sur les pages, le deuxième terme permet du nom de l'image permet de créer de lister les œuvres en plusieurs groupes (ex: raku-Vases+vase-rouge-bombé+principal+yasefanprod). Il est aussi possible d'afficher des photos de stages par date (ex: stages-jeudi-30-février-2017+groupe+principal).

<div>
{% cloudinary /assets/casestudies/jekyll-for-craftman-collections.png alt="Jekyll - Un thème pour artisans" %}
</div>

