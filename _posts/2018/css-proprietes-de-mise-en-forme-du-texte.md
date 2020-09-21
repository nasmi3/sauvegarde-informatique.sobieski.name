---
ID: 14
post_title: '[CSS] Propriétés de mise en forme du texte'
post_name: css-proprietes-de-mise-en-forme-du-texte
author: Alexandre
post_date: 2018-03-26 10:04:41
layout: post
link: >
  http://sobieski.name/informatique/css/css-proprietes-de-mise-en-forme-du-texte/
published: true
tags: [ ]
categories:
  - CSS
---
Je résume ici la plupart des propriétés de mise en forme du texte.

Qu'est-ce que la mise en forme de texte ? C'est tout ce qui touche à la présentation du texte proprement dit : le <strong>gras</strong>, l'<em>italique</em>, le <u>souligné</u>, la police, l'alignement, etc.
<h2 id="table-des-matières-nocount-ignoretrue">Table des matières</h2>
<!-- @import "[TOC]" {cmd="toc" depthFrom=2 depthTo=6 orderedList=true} -->
<!-- code_chunk_output -->
<ol>
 	<li><a href="#modifications-des-caractères">Modifications des caractères</a></li>
 	<li><a href="#propriétés-de-couleur-et-de-fond">Propriétés de couleur et de fond</a></li>
 	<li><a href="#propriétés-des-boîtes">Propriétés des boîtes</a></li>
 	<li><a href="#propriétés-de-positionnement-et-daffichage">Propriétés de positionnement et d'affichage</a></li>
 	<li><a href="#propriétés-des-listes">Propriétés des listes</a></li>
 	<li><a href="#propriétés-des-tableaux">Propriétés des tableaux</a></li>
 	<li><a href="#autres-propriétés">Autres propriétés</a></li>
</ol>
<!-- /code_chunk_output -->
<h2 id="modifications-des-caractères">Modifications des caractères</h2>
<table>
<thead>
<tr>
<th style="text-align: center;">Propriété</th>
<th>Valeurs (exemples)</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="language-css css">font-family</code></td>
<td>police1, police2, police3, serif, sans-serif, monospace</td>
<td>Nom de police</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">@font-face</code></td>
<td>Nom et source de la police</td>
<td>Police personnalisée</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">font-size</code></td>
<td>1.3em, 16px, 120%…</td>
<td>Taille du texte</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">font-weight</code></td>
<td>bold, normal</td>
<td>Gras</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">font-style</code></td>
<td>italic, oblique, normal</td>
<td>Italique</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">text-decoration</code></td>
<td>underline, overline, line-through, blink, none</td>
<td>Soulignement, ligne au-dessus, barré ou clignotant</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">font-variant</code></td>
<td>small-caps, normal</td>
<td>Petites capitales</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">text-transform</code></td>
<td>capitalize, lowercase, uppercase</td>
<td>Capitales</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">font</code></td>
<td>-</td>
<td>Super propriété de police. Combine : font-weight,font-style, font-size, font-variant, font-family.</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">text-align</code></td>
<td>left, center, right, justify</td>
<td>Alignement horizontal</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">vertical-align</code></td>
<td>baseline, middle, sub, super, top, bottom</td>
<td>Alignement vertical (cellules de tableau ou élémentsinline-block uniquement)</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">line-height</code></td>
<td>18px, 120%, normal…</td>
<td>Hauteur de ligne</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">text-indent</code></td>
<td>25px</td>
<td>Alinéa</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">white-space</code></td>
<td>pre, nowrap, normal</td>
<td>Césure</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">word-wrap</code></td>
<td>break-word, normal</td>
<td>Césure forcée</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">text-shadow</code></td>
<td>5px 5px 2px blue</td>
<td></td>
</tr>
<tr>
<td style="text-align: center;">(horizontale, verticale, fondu, couleur)</td>
<td>Ombre de texte</td>
<td></td>
</tr>
</tbody>
</table>
<h2 id="propriétés-de-couleur-et-de-fond">Propriétés de couleur et de fond</h2>
<table>
<thead>
<tr>
<th style="text-align: center;">Propriété</th>
<th>Valeurs (exemples)</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="language-css css">color</code></td>
<td>nom, rgb(rouge,vert,bleu), rgba(rouge,vert,bleu,transparence), #CF1A20…</td>
<td>Couleur du texte</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">background-color</code></td>
<td>Identique à color</td>
<td>Couleur de fond</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">background-image</code></td>
<td>url('image.png')</td>
<td>Image de fond</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">background-attachment</code></td>
<td>fixed, scroll</td>
<td>Fond fixe</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">background-repeat</code></td>
<td>repeat-x, repeat-y, no-repeat, repeat</td>
<td>Répétition du fond</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">background-position</code></td>
<td>(x y), top, center, bottom, left, right</td>
<td>Position du fond</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">background</code></td>
<td>-</td>
<td>Super propriété du fond. Combine :<code class="language-css css">background-image</code>, <code class="language-css css">background-repeat</code>,<code class="language-css css">background-attachment</code>, <code class="language-css css">background-position</code></td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">opacity</code></td>
<td>0.5</td>
<td>Transparence</td>
</tr>
</tbody>
</table>
<h2 id="propriétés-des-boîtes">Propriétés des boîtes</h2>
<table>
<thead>
<tr>
<th style="text-align: center;">Propriété</th>
<th>Valeurs (exemples)</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="language-css css">width</code></td>
<td>150px, 80%…</td>
<td>Largeur</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">height</code></td>
<td>150px, 80%…</td>
<td>Hauteur</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">min-width</code></td>
<td>150px, 80%…</td>
<td>Largeur minimale</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">max-width</code></td>
<td>150px, 80%…</td>
<td>Largeur maximale</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">min-height</code></td>
<td>150px, 80%…</td>
<td>Hauteur minimale</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">max-height</code></td>
<td>150px, 80%…</td>
<td>Hauteur maximale</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">margin-top</code></td>
<td>23px</td>
<td>Marge en haut</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">margin-left</code></td>
<td>23px</td>
<td>Marge à gauche</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">margin-right</code></td>
<td>23px</td>
<td>Marge à droite</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">margin-bottom</code></td>
<td>23px</td>
<td>Marge en bas</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">margin</code></td>
<td>23px 5px 23px 5px (haut, droite, bas, gauche)</td>
<td>Super-propriété de marge. Combine : margin-top, margin-right, margin-bottom, margin-left</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">padding-left</code></td>
<td>23px</td>
<td>Marge intérieure à gauche</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">padding-right</code></td>
<td>23px</td>
<td>Marge intérieure à droite</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">padding-bottom</code></td>
<td>23px</td>
<td>Marge intérieure en bas</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">padding-top</code></td>
<td>23px</td>
<td>Marge intérieure en haut</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">padding</code></td>
<td>23px 5px 23px 5px (haut, droite, bas, gauche)</td>
<td>Super-propriété de marge intérieure.</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">border-width</code></td>
<td>3px</td>
<td>Épaisseur de bordure</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">border-color</code></td>
<td>nom, rgb(rouge,vert,bleu), rgba(rouge,vert,bleu,transparence), #CF1A20…</td>
<td>Couleur de bordure</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">border-style</code></td>
<td>solid, dotted, dashed, double, groove, ridge, inset, outset</td>
<td>Type de bordure</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">border</code></td>
<td>3px solid black</td>
<td>Super-propriété de bordure. Combine border-width, border-color, border-style. Existe aussi en version border-top, border-right, border-bottom, border-left.</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">border-radius</code></td>
<td>5px</td>
<td>Bordure arrondie</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">box-shadow</code></td>
<td>6px 6px 0px black (horizontale, verticale, fondu, couleur)</td>
<td>Ombre de boîte</td>
</tr>
</tbody>
</table>
<h2 id="propriétés-de-positionnement-et-daffichage">Propriétés de positionnement et d'affichage</h2>
<table>
<thead>
<tr>
<th style="text-align: center;">Propriété</th>
<th>Valeurs (exemples)</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="language-css css">display</code></td>
<td>block, inline, inline-block, table, table-cell, none…</td>
<td>Type d'élément (block, inline, inline-block,none…)</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">visibility</code></td>
<td>visible, hidden</td>
<td>Visibilité</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">clip</code></td>
<td>rect (0px, 60px, 30px, 0px)</td>
<td></td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">rect</code></td>
<td>(haut, droite, bas, gauche)</td>
<td>Affichage d'une partie de l'élément</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">overflow</code></td>
<td>auto, scroll, visible, hidden</td>
<td>Comportement en cas de dépassement</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">float</code></td>
<td>left, right, none</td>
<td>Flottant</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">clear</code></td>
<td>left, right, both, none</td>
<td>Arrêt d'un flottant</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">position</code></td>
<td>relative, absolute, static</td>
<td>Positionnement</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">top</code></td>
<td>20px</td>
<td>Position par rapport au haut</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">bottom</code></td>
<td>20px</td>
<td>Position par rapport au bas</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">left</code></td>
<td>20px</td>
<td>Position par rapport à la gauche</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">right</code></td>
<td>20px</td>
<td>Position par rapport à la droite</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">z-index</code></td>
<td>10</td>
<td>Ordre d'affichage en cas de superposition. La plus grande valeur est affichée par-dessus les autres.</td>
</tr>
</tbody>
</table>
<h2 id="propriétés-des-listes">Propriétés des listes</h2>
<table>
<thead>
<tr>
<th style="text-align: center;">Propriété</th>
<th>Valeurs (exemples)</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="language-css css">list-style-type</code></td>
<td>disc, circle, square, decimal, lower-roman, upper-roman, lower-alpha, upper-alpha, none</td>
<td>Type de liste</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">list-style-position</code></td>
<td>inside, outside</td>
<td>Position en retrait</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">list-style-image</code></td>
<td>url('puce.png')</td>
<td>Puce personnalisée</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">list-style</code></td>
<td>-</td>
<td>Super-propriété de liste. Combine list-style-type, list-style-position, list-style-image.</td>
</tr>
</tbody>
</table>
<h2 id="propriétés-des-tableaux">Propriétés des tableaux</h2>
<table>
<thead>
<tr>
<th style="text-align: center;">Propriété</th>
<th>Valeurs (exemples)</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="language-css css">border-collapse</code></td>
<td>collapse, separate</td>
<td>Fusion des bordures</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">empty-cells</code></td>
<td>hide, show</td>
<td>Affichage des cellules vides</td>
</tr>
<tr>
<td style="text-align: center;"><code class="language-css css">caption-side</code></td>
<td>bottom, top</td>
<td>Position du titre du tableau</td>
</tr>
</tbody>
</table>
<h2 id="autres-propriétés">Autres propriétés</h2>
<table>
<thead>
<tr>
<th style="text-align: center;">Propriété</th>
<th>Valeurs (exemple)</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="language-css css">cursor</code></td>
<td>crosshair, default, help, move, pointer, progress, text, wait, e-resize, ne-resize, auto…</td>
<td>Curseur de souris</td>
</tr>
</tbody>
</table>