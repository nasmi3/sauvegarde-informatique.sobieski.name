---
ID: 18
post_title: '[SQL] Fiche de synthèse SQL'
post_name: sql-fiche-de-synthese-sql
author: Alexandre
post_date: 2018-03-25 22:18:08
layout: post
link: >
  http://sobieski.name/informatique/sql/sql-fiche-de-synthese-sql/
published: true
tags: [ ]
categories:
  - SQL
---
<h2 id="table-des-matières">Table des matières</h2>
<!-- @import "[TOC]" {cmd="toc" depthFrom=2 depthTo=6 orderedList=false} -->
<!-- code_chunk_output -->
<ul>
 	<li><a href="#syntaxe">Syntaxe</a></li>
 	<li><a href="#créer-une-table">Créer une table</a></li>
 	<li><a href="#insérer-des-valeurs-dans-une-table">Insérer des valeurs dans une table</a></li>
 	<li><a href="#sélectionner-des-valeurs-dune-table">Sélectionner des valeurs d’une table</a></li>
 	<li><a href="#éditer-une-ligne">Éditer une ligne</a></li>
 	<li><a href="#modifier-un-tableau">Modifier un tableau</a></li>
 	<li><a href="#supprimer-une-ligne">Supprimer une ligne</a></li>
</ul>
<!-- /code_chunk_output -->
<h2 id="syntaxe">Syntaxe</h2>
Chaque commande est composée d’une clause qui est la fonction qui sera appliquée (on l’écrit en majuscules), puis d’une référence pour savoir à quoi s’applique cette fonction et pour finir d’éventuels paramètres entre parenthèses séparés par des virgues <code class="sql language-sql">,</code>.

Toute commande est terminée par un point-virgule<code class="sql language-sql">;</code>.

<strong>Exemple :</strong>
<pre><code class="sql language-sql">CREATE TABLE table_name (
column_1 data_type,
column_2 data_type,
column_3 data_type
);</code></pre>
<h2 id="créer-une-table">Créer une table</h2>
On utilise la commande <code class="sql language-sql">CREATE TABLE</code>. On indique le nom de la table en référence et les couples <code class="sql language-sql">nom_de_colonne</code> – <code class="sql language-sql">type</code> qui composent sa structure interne.

<strong>Exemple :</strong>
<pre><code class="sql language-sql">CREATE TABLE nom_table (id INTEGER, col_2 TEXT, col_3 INTEGER);</code></pre>
<h2 id="insérer-des-valeurs-dans-une-table">Insérer des valeurs dans une table</h2>
On utilise la commande <code class="sql language-sql">INSERT INTO</code> avec pour référence la table dans laquelle on inscrit les valeurs (après avoir indiqué les colonnes à remplir) et on indique les valeurs avec <code class="sql language-sql">VALUES</code> et les <code class="sql language-sql">n-uplets</code> correspondants en paramètre.

<strong>Exemple :</strong>
<pre><code class="sql language-sql">INSERT INTO table (id, name, age) VALUES (1, "Freddy Mercury", 21);</code></pre>
<strong><em>Q : Peut-on mettre plusieurs couples en une seule commande ?</em></strong>
<h2 id="sélectionner-des-valeurs-d’une-table">Sélectionner des valeurs d’une table</h2>
On utilise ici <code class="sql language-sql">SELECT</code>. Il suffit d’indiquer la provenance des données lues avec l’instruction <code class="sql language-sql">FROM</code>.

<strong>Exemple :</strong>
<pre><code class="sql language-sql">SELECT name FROM base_clients;</code></pre>
La commande <code class="sql language-sql">WHERE</code> (conditions) est utilisée pour définir les lignes à modifier. On peut utiliser <code class="sql language-sql">WHERE paramètre = valeur</code> ou <code class="sql language-sql">WHERE paramètre IS valeur</code>.
<h2 id="éditer-une-ligne">Éditer une ligne</h2>
On utilise la commande <code class="sql language-sql">UPDATE</code> avec le nom de la table et <code class="sql language-sql">SET</code> pour indiquer quelle est la nouvelle valeur.

<strong>Exemple :</strong>
<pre><code class="sql language-sql">UPDATE celebs
SET age = 22
WHERE id = 1;

SELECT * FROM celebs;</code></pre>
<h2 id="modifier-un-tableau">Modifier un tableau</h2>
On utilise la commande <code class="sql language-sql">ALTER TABLE</code> pour modifier la table d’une base de données.

L’instruction <code class="sql language-sql">ADD COLUMN</code> permet comme son nom l’indique de rajouter une colonne à la table.

Il faut ajouter le nom et le type de données contenus dans la colonne. Toutes les lignes déjà remplies contiennent par défaut la valeur <code class="sql language-sql">NULL</code>.

<strong>Exemple :</strong>
<pre><code class="sql language-sql">ALTER TABLE tableau ADD COLUMN twitter_url TEXT;</code></pre>
<h2 id="supprimer-une-ligne">Supprimer une ligne</h2>
On utilise l’instruction <code class="sql language-sql">DELETE</code> suivi d’une sélection.

<strong>Exemple :</strong>
<pre><code class="sql language-sql">DELETE FROM tableau WHERE twitter_url IS NULL;</code></pre>