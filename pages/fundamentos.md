---
layout: default
permalink: /13-principios/
title: "13 Principios de fe"
---

En su influyente **Comentario a la Mishná** (Tratado Sanhedrín 10), el gran sabio Rabí Moshé ben Maimón, conocido como **Maimónides** (o el **Rambam**), articuló los **Trece Principios de la Fe Judía** (*Ikarei HaEmuná*). Estos principios se han convertido en la base doctrinal del judaísmo a lo largo de los siglos.

A continuación, exploramos el texto y la esencia de los **fundamentos** de la fe.

## Principios sobre D-s
* La Existencia de D-s (Metziut HaShem): Creer que existe un Creador, la Causa de todo.

* La Unidad de D-s (Yijúd HaShem): Creer que D-s es uno en una unidad sin paralelo.

* La Incorporeidad de D-s (She'Ein Lo Guf): Creer que D-s no es físico, no tiene cuerpo ni forma.

* La Eternidad de D-s (Kidmut HaShem): Creer que D-s es el primero y el último, y que es eterno.

* Solo a D-s se Debe Rezar (Tefilah Le'HaShem Levadó): Creer que solo a D-s se debe dirigir el culto y la oración.

## Principios sobre la Profecía y Revelación
* La Verdad de la Profecía (Nevuáh): Creer que D-s se comunica con los humanos a través de la profecía.

* La Supremacía de Moshé (Nevu'at Moshé): Creer que la profecía de Moshé (Moisés) fue la mayor y más verdadera de todas.

* La Inmutabilidad de la Torá (Torat Moshé): Creer que la Torá que tenemos hoy es exactamente la que le fue entregada a Moshé, y que nunca será cambiada.

Principios sobre la Retribución
* La Permanencia de la Torá (Lo Titjádef): Creer que la Torá (la de Moshé) nunca será reemplazada o abolida por otra.

* La Omnisciencia de D-s (Yedi'at HaShem): Creer que D-s conoce los pensamientos y las acciones de los humanos (Su providencia).

* La Recompensa y el Castigo (Shjájar Va'Onesh): Creer que D-s recompensa a los que cumplen Sus mandamientos y castiga a los que los transgreden.

## Principios sobre la Redención
* La Venida del Mashíaj (Bi'at HaMashíaj): Creer en la llegada del Mesías, y aunque se demore, debemos esperar Su venida todos los días.

* La Resurrección de los Muertos (Tjiyat HaMetim): Creer que habrá una resurrección de los muertos en el futuro.

-------------------

# Posts
<div>

<ul>
  {% for post in site.posts %}

    {% if post.category == 'fundamentos' %}
      <li>
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endif %}

  {% endfor %}
</ul>

</div>
