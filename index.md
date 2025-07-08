---
layout: page
list_title: Dernières nouvelles
n_posts: 8
n_news: 1
n_actus: 2
---

# Bienvenue sur le réseau de la recherche reproductible

> Pour un chercheur, il n’y a rien de plus frustrant que l’impossibilité de reproduire des résultats majeurs obtenus quelques mois auparavant. Les causes de ce type de déconvenues sont multiples et parfois pernicieuses. Ce phénomène participe à ce que certains identifient comme une “crise de la reproductibilité de la recherche”. --- Vers une recherche reproductible, Desquilbet et al., 2019.

<!--
![Actions reseau](../assets/images/banniere_web.png){: style="width: 50%; display:block; margin-right: auto; margin-left:auto;" }
-->

## News !

<div class="news">
<h6>  Wébinaires </h6>
  <ul class="post-list">
   {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
     {%- for post in site.categories.webinaires limit:page.n_news -%}
      <li>
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
      </li>
   {%- endfor -%}
  </ul>
  <ul class="post-list">
   {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
     {%- for post in site.categories.past-webinaires limit:page.n_news -%}
      <li>
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
      </li>
   {%- endfor -%}
  </ul>


<h6>Conférences </h6>
<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.event limit:page.n_news -%}
    <li>
      <span class="post-meta">{{ post.date | date: date_format }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h3>
    </li>
 {%- endfor -%}
</ul>

<h6>Actualités du réseau</h6>

{% if site.paginate %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.news limit:page.n_actus -%}
    <li>
      <span class="post-meta">{{ post.date | date: date_format }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h3>
    </li>
 {%- endfor -%}
</ul>

<h6>Divers</h6>

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.newsletter limit:page.n_news -%}
    <li>
      <span class="post-meta">{{ post.date | date: date_format }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h3>
    </li>
 {%- endfor -%}
</ul>


La prochaine newsletter est en préparation, n'hésitez pas à nous faire part des contenus que vous voudriez partager avec la communauté !

<div class="news2"> Retrouvez l'intégralité des actualités <a href="{{activities | relative_url}}/activities/">sur cette page</a> !</div>
</div>


<br>
# Le réseau

Le Réseau Français de la Recherche Reproductible est une initiative nationale informelle rassemblant des scientifiques engagés dans l’étude des facteurs favorisant la reproductibilité de la recherche. Bien que les enjeux de la reproductibilité varient selon les disciplines, ils concernent l’ensemble des domaines scientifiques. Le réseau s’attache ainsi à représenter une diversité disciplinaire riche et équilibrée. 
[Plus d'information dans ce document !](assets/pdfs/presentation.pdf)


## Objectifs du réseau
L’objectif du réseau est de contribuer à modifier les pratiques de recherche pour les rendre plus reproductibles, plus robustes et plus transparentes. 

  <p>Il s’agit donc :</p>
  <ul>
    <li>Créer une communauté multidisciplinaire engagée à promouvoir la reproductibilité des recherches scientifiques ;</li>
    <li>Identifier les défis pour la reproductibilité des résultats de recherche et définir des actions concrètes pour améliorer cette situation dans différentes disciplines, notamment la mise en place et la diffusion de bonnes pratiques, la formation, et l'acculturation des chercheur·euse·s ;</li>
    <li>Étendre cette dynamique à l'échelle institutionnelle, nationale et internationale, tout en établissant des connexions avec les initiatives liées à la science ouverte et à l'intégrité scientifique.</li>
  </ul>


![Objectifs réseau](../assets/images/objectifs_recherche-repro-fr.png){: style="width: 55%; display:block; margin-right: auto; margin-left:auto;" }

## Actions en cours

![Actions reseau](../assets/images/activites_recherche-repro.png){: style="width: 60%; display:block; margin-right: auto; margin-left:auto;" }

## Comment contribuer ?

La reproductibilité est un sujet qui vous intéresse ? 

<p> Vous pouvez : </p>
<ul>
    <li>vous abonner à <a href="https://groupes.renater.fr/sympa/info/recherche-reproductible" target="_blank">la liste de diffusion</a> pour être informé </li>
    <li>diffuser des informations dans vos réseaux professionnels : relayer les mails, mettre une affiche, … </li>
    <li>animer une sensibilisation dans votre laboratoire ou mettre en place un ReproducibiliTea </li>
    <li>proposer une sensibilisation aux doctorants de votre école doctorale </li>
    <li>rédiger une fiche de bonnes pratiques spécifiques à votre discipline </li>
    <li>participer à <a href="https://www.recherche-reproductible.fr/steering/" target="_blank"> un groupe de travail ou un collège</a>></li>
    <li> proposer un nouveau groupe de travail</li>
 </ul>

N’hésitez pas à nous rejoindre !

<br/>
<a href="https://groupes.renater.fr/sympa/info/recherche-reproductible" target="_blank">![Actions reseau](../assets/images/Contacts.png){: style="width: 65%; display:block; margin-right: auto; margin-left:auto;" }</a>
