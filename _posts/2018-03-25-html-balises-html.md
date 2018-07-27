---
ID: 16
post_title: '[HTML] Balises HTML'
author: Alexandre
post_excerpt: ""
layout: post
permalink: >
  http://sobieski.name/informatique/html/html-balises-html/
published: true
post_date: 2018-03-25 23:20:29
tags: [ ]
categories:
  - HTML
---
<h2 id="table-des-matières-nocount-ignoretrue">Table des matières</h2>
<!-- @import "[TOC]" {cmd="toc" depthFrom=2 depthTo=6 orderedList=true} -->
<!-- code_chunk_output -->
<ol>
 	<li><a href="#balises-de-premier-niveau">Balises de premier niveau</a></li>
 	<li><a href="#balises-den-tête">Balises d'en-tête</a></li>
 	<li><a href="#balises-de-structuration-du-texte">Balises de structuration du texte</a></li>
 	<li><a href="#balises-de-listes">Balises de listes</a></li>
 	<li><a href="#balises-de-tableau">Balises de tableau</a></li>
 	<li><a href="#balises-de-formulaire">Balises de formulaire</a></li>
 	<li><a href="#balises-sectionnantes">Balises sectionnantes</a></li>
 	<li><a href="#balises-génériques">Balises génériques</a></li>
</ol>
<!-- /code_chunk_output -->
<h2 id="balises-de-premier-niveau">Balises de premier niveau</h2>
Les balises de premier niveau sont les principales balises qui structurent une page HTML. Elles sont indispensables pour réaliser le « code minimal » d'une page web.
<table>
<thead>
<tr>
<th style="text-align: center;">Balise</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;html&gt;</code></td>
<td>Balise principale</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;head&gt;</code></td>
<td>En-tête de la page</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;body&gt;</code></td>
<td>Corps de la page</td>
</tr>
</tbody>
</table>
Code minimal d'une page HTML :
<pre><code class="html language-html">&lt;!DOCTYPE html&gt;
&lt;html&gt;
    &lt;head&gt;
        &lt;meta charset="utf-8" /&gt;
        &lt;title&gt;Titre&lt;/title&gt;
    &lt;/head&gt;

    &lt;body&gt;

    &lt;/body&gt;
&lt;/html&gt;</code></pre>

<hr />

<h2 id="balises-den-tête">Balises d'en-tête</h2>
Ces balises sont toutes situées dans l'en-tête de la page web, c'est-à-dire entre <code class="html language-html">&lt;head&gt;</code> et <code class="html language-html">&lt;/head&gt;</code> :
<table>
<thead>
<tr>
<th style="text-align: center;">Balise</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;link/&gt;</code></td>
<td>Liaison avec une feuille de style</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;meta/&gt;</code></td>
<td>Métadonnées de la page web (charset, mots-clés, etc.)</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;script&gt;</code></td>
<td>Code JavaScript</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;style&gt;</code></td>
<td>Code CSS</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;title&gt;</code></td>
<td>Titre de la page</td>
</tr>
</tbody>
</table>

<hr />

<h2 id="balises-de-structuration-du-texte">Balises de structuration du texte</h2>
<table>
<thead>
<tr>
<th style="text-align: center;">Balise</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;abbr&gt;</code></td>
<td>Abréviation</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;blockquote&gt;</code></td>
<td>Citation (longue)</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;cite&gt;</code></td>
<td>Citation du titre d'une œuvre ou d'un évènement</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;q&gt;</code></td>
<td>Citation (courte)</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;sup&gt;</code></td>
<td>Exposant</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;sub&gt;</code></td>
<td>Indice</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;strong&gt;</code></td>
<td>Mise en valeur forte</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;em&gt;</code></td>
<td>Mise en valeur normale</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;mark&gt;</code></td>
<td>Mise en valeur visuelle</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;h1&gt;</code></td>
<td>Titre de niveau 1</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;h2&gt;</code></td>
<td>Titre de niveau 2</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;h3&gt;</code></td>
<td>Titre de niveau 3</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;h4&gt;</code></td>
<td>Titre de niveau 4</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;h5&gt;</code></td>
<td>Titre de niveau 5</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;h6&gt;</code></td>
<td>Titre de niveau 6</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;img/&gt;</code></td>
<td>Image</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;figure&gt;</code></td>
<td>Figure (image, code, etc.)</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;figcaption&gt;</code></td>
<td>Description de la figure</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;audio&gt;</code></td>
<td>Son</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;video&gt;</code></td>
<td>Vidéo</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;source&gt;</code></td>
<td>Format source pour les balises <code class="html language-html">&lt;audio&gt;</code> et <code class="html language-html">&lt;video&gt;</code></td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;a&gt;</code></td>
<td>Lien hypertexte</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;br/&gt;</code></td>
<td>Retour à la ligne</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;p&gt;</code></td>
<td>Paragraphe</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;hr/&gt;</code></td>
<td>Ligne de séparation horizontale</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;address&gt;</code></td>
<td>Adresse de contact</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;del&gt;</code></td>
<td>Texte supprimé</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;ins&gt;</code></td>
<td>Texte inséré</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;dfn&gt;</code></td>
<td>Définition</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;kbd&gt;</code></td>
<td>Saisie clavier</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;pre&gt;</code></td>
<td>Affichage formaté (pour les codes sources)</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;progress&gt;</code></td>
<td>Barre de progression</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;time&gt;</code></td>
<td>Date ou heure</td>
</tr>
</tbody>
</table>

<hr />

<h2 id="balises-de-listes">Balises de listes</h2>
Cette section énumère toutes les balises <code class="html language-html">HTML</code> permettant de créer des listes (listes à puces, listes numérotées, listes de définitions…)
<table>
<thead>
<tr>
<th style="text-align: center;">Balise</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;ul&gt;</code></td>
<td>Liste à puces, non numérotée</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;ol&gt;</code></td>
<td>Liste numérotée</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;li&gt;</code></td>
<td>Élément de la liste à puces</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;dl&gt;</code></td>
<td>Liste de définitions</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;dt&gt;</code></td>
<td>Terme à définir</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;dd&gt;</code></td>
<td>Définition du terme</td>
</tr>
</tbody>
</table>

<hr />

<h2 id="balises-de-tableau">Balises de tableau</h2>
<table>
<thead>
<tr>
<th style="text-align: center;">Balise</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;table&gt;</code></td>
<td>Tableau</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;caption&gt;</code></td>
<td>Titre du tableau</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;tr&gt;</code></td>
<td>Ligne de tableau</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;th&gt;</code></td>
<td>Cellule d'en-tête</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;td&gt;</code></td>
<td>Cellule</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;thead&gt;</code></td>
<td>Section de l'en-tête du tableau</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;tbody&gt;</code></td>
<td>Section du corps du tableau</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;tfoot&gt;</code></td>
<td>Section du pied du tableau</td>
</tr>
</tbody>
</table>

<hr />

<h2 id="balises-de-formulaire">Balises de formulaire</h2>
<table>
<thead>
<tr>
<th style="text-align: center;">Balise</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;form&gt;</code></td>
<td>Formulaire</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;fieldset&gt;</code></td>
<td>Groupe de champs</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;legend&gt;</code></td>
<td>Titre d'un groupe de champs</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;label&gt;</code></td>
<td>Libellé d'un champ</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;input/&gt;</code></td>
<td>Champ de formulaire (texte, mot de passe, case à cocher, bouton, etc.)</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;textarea&gt;</code></td>
<td>Zone de saisie multiligne</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;select&gt;</code></td>
<td>Liste déroulante</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;option&gt;</code></td>
<td>Élément d'une liste déroulante</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;optgroup&gt;</code></td>
<td>Groupe d'éléments d'une liste déroulante</td>
</tr>
</tbody>
</table>

<hr />

<h2 id="balises-sectionnantes">Balises sectionnantes</h2>
Ces balises permettent de construire le squelette de notre site web.
<table>
<thead>
<tr>
<th style="text-align: center;">Balise</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;header&gt;</code></td>
<td>En-tête</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;nav&gt;</code></td>
<td>Liens principaux de navigation</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;footer&gt;</code></td>
<td>Pied de page</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;section&gt;</code></td>
<td>Section de page</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;article&gt;</code></td>
<td>Article (contenu autonome)</td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;aside&gt;</code></td>
<td>Informations complémentaires</td>
</tr>
</tbody>
</table>

<hr />

<h2 id="balises-génériques">Balises génériques</h2>
Les balises génériques sont des balises qui n'ont pas de sens sémantique.

En effet, toutes les autres balises HTML ont un sens : <code class="html language-html">&lt;p&gt;</code> signifie « Paragraphe », <code class="html language-html">&lt;h2&gt;</code> signifie « Sous-titre », etc.

Parfois, on a besoin d'utiliser des balises génériques (aussi appelées balises universelles) car aucune des autres balises ne convient. On utilise le plus souvent des balises génériques pour construire son design.
Il y a deux balises génériques : l'une est <code class="html language-html">inline</code>, l'autre est <code class="html language-html">block</code>.
<table>
<thead>
<tr>
<th style="text-align: center;">Balise</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;span&gt;</code></td>
<td>Balise générique de type <code class="html language-html">inline</code></td>
</tr>
<tr>
<td style="text-align: center;"><code class="html language-html">&lt;div&gt;</code></td>
<td>Balise générique de type <code class="html language-html">block</code></td>
</tr>
</tbody>
</table>
Ces balises ont un intérêt uniquement si vous leur associez un attribut <code class="html language-html">class</code>, <code class="html language-html">id</code> ou <code class="html language-html">style</code> :
<ul>
 	<li><code class="html language-html">class</code>: indique le nom de la classe CSS à utiliser.</li>
 	<li><code class="html language-html">id</code>: donne un nom à la balise. Ce nom doit être unique sur toute la page car il permet d'identifier la balise. Vous pouvez vous servir de l'ID pour de nombreuses choses, par exemple pour créer un lien vers une ancre, pour un style CSS de type ID, pour des manipulations en JavaScript, etc.</li>
 	<li><code class="html language-html">style</code>: cet attribut vous permet d'indiquer directement le code CSS à appliquer. Vous n'êtes donc pas obligés d'avoir une feuille de style à part, vous pouvez mettre directement les attributs CSS. Notez qu'il est préférable de ne pas utiliser cet attribut et de passer à la place par une feuille de style externe, car cela rend votre site plus facile à mettre à jour par la suite.
Ces trois attributs ne sont pas réservés aux balises génériques : vous pouvez aussi les utiliser sans aucun problème dans la plupart des autres balises.</li>
</ul>