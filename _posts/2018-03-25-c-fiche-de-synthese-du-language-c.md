---
ID: 12
post_title: '[C#] Fiche de synthèse du language C#'
author: Alexandre
post_excerpt: ""
layout: post
permalink: >
  http://sobieski.name/informatique/c/c-fiche-de-synthese-du-language-c/
published: true
post_date: 2018-03-25 23:56:51
tags: [ ]
categories:
  - 'C#'
---
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
<!-- code_chunk_output -->
<ul>
 	<li><a href="#c-fiche-de-synthèse-du-language-c">[C#] Fiche de synthèse du language C#</a>
<ul>
 	<li><a href="#remarques">Remarques</a></li>
 	<li><a href="#commenter-une-ligne">Commenter une ligne</a></li>
 	<li><a href="#types-de-variables">Types de variables :</a></li>
 	<li><a href="#opérations">Opérations</a>
<ul>
 	<li><a href="#mathématiques">Mathématiques</a>
<ul>
 	<li><a href="#les-classiques">Les classiques :</a></li>
 	<li><a href="#les-spéciales">Les spéciales :</a></li>
 	<li><a href="#les-condensées">Les condensées :</a></li>
</ul>
</li>
 	<li><a href="#les-chaines-de-caractère">Les chaines de caractère</a>
<ul>
 	<li><a href="#astuces">Astuces :</a></li>
</ul>
</li>
 	<li><a href="#opérateurs-de-comparaison">Opérateurs de comparaison</a>
<ul>
 	<li><a href="#de-booléens">De booléens</a></li>
 	<li><a href="#de-nombres">De nombres</a></li>
</ul>
</li>
</ul>
</li>
 	<li><a href="#les-boucles">Les boucles</a>
<ul>
 	<li><a href="#if">If</a></li>
 	<li><a href="#case">case</a></li>
 	<li><a href="#for">For</a></li>
 	<li><a href="#foreach">Foreach</a></li>
 	<li><a href="#while">While</a>
<ul>
 	<li><a href="#alternative">Alternative</a></li>
</ul>
</li>
 	<li><a href="#break-et-continue">Break et continue</a>
<ul>
 	<li><a href="#break">Break</a></li>
 	<li><a href="#continue">Continue</a></li>
</ul>
</li>
</ul>
</li>
 	<li><a href="#les-blocs-de-code">Les blocs de code</a></li>
 	<li><a href="#les-méthodes-ou-fonctions">Les "méthodes" ou fonctions</a>
<ul>
 	<li><a href="#descripteurs">Descripteurs</a></li>
 	<li><a href="#valeur-de-retour">Valeur de retour</a></li>
</ul>
</li>
 	<li><a href="#les-ensembles-de-données">Les ensembles de données</a>
<ul>
 	<li><a href="#les-tableaux">Les tableaux</a>
<ul>
 	<li><a href="#création-dun-tableau">Création d'un tableau</a></li>
 	<li><a href="#syntaxe">Syntaxe</a></li>
</ul>
</li>
 	<li><a href="#les-listes">Les listes</a>
<ul>
 	<li><a href="#outils">Outils</a></li>
</ul>
</li>
 	<li><a href="#les-énumérations">Les énumérations</a></li>
</ul>
</li>
 	<li><a href="#le-framework-net">Le framework .NET</a></li>
 	<li><a href="#conversion-entre-les-types-de-données">Conversion entre les types de données</a>
<ul>
 	<li><a href="#directement">Directement</a></li>
 	<li><a href="#conversion-explicite">Conversion explicite</a></li>
 	<li><a href="#entre-types-incompatibles">Entre types incompatibles</a></li>
</ul>
</li>
 	<li><a href="#interactions-avec-lutilisateur">Interactions avec l’utilisateur</a>
<ul>
 	<li><a href="#récupérer-un-texte">Récupérer un texte</a></li>
 	<li><a href="#lecture-dun-caractère">Lecture d’un caractère</a></li>
</ul>
</li>
 	<li><a href="#programmation-orientée-objet">Programmation orientée objet</a>
<ul>
 	<li><a href="#encapsulation">Encapsulation</a></li>
 	<li><a href="#héritage">Héritage</a></li>
 	<li><a href="#polymorphisme">Polymorphisme</a></li>
 	<li><a href="#substitution">Substitution</a></li>
</ul>
</li>
</ul>
</li>
</ul>
<!-- /code_chunk_output -->
<h2 id="remarques">Remarques</h2>
Sensibles à la casse, toutes les instructions se terminent avec un <code class="csharp language-csharp">;</code>
<h2 id="commenter-une-ligne">Commenter une ligne</h2>
Sur la même ligne / à la fin d'une ligne : avec <code class="csharp language-csharp">//</code>
Sur plusieurs lignes : <code class="csharp language-csharp">/*</code> et pour terminer <code class="csharp language-csharp">*/</code>
<h2 id="types-de-variables-">Types de variables :</h2>
<table>
<thead>
<tr>
<th style="text-align: center;">Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">byte</code></td>
<td>Entier de 0 à 255</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">short</code></td>
<td>Entier de -32768 à 32767</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">int</code></td>
<td>Entier de -2147483648 à 2147483647</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">long</code></td>
<td>Entier de -9223372036854775808 à 9223372036854775807</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">float</code></td>
<td>Nombre simple précision de -3,402823e38 à 3,402823e38</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">double</code></td>
<td>Nombre double précision de -1,79769313486232 e308 à 1,79769313486232 e308</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">decimal</code></td>
<td>Nombre décimal convenant particulièrement aux calculs financiers</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">char</code></td>
<td>Représente un caractère</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">string</code></td>
<td>Une chaîne de caractère</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">bool</code></td>
<td>Une valeur booléenne (vrai ou faux)</td>
</tr>
</tbody>
</table>
<h2 id="opérations">Opérations</h2>
<h3 id="mathématiques">Mathématiques</h3>
<h4 id="les-classiques-">Les classiques :</h4>
<table>
<thead>
<tr>
<th style="text-align: center;">Symbole</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">+</code></td>
<td>Addition</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">-</code></td>
<td>Soustraction</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">*</code></td>
<td>Produit</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">/</code></td>
<td>Division</td>
</tr>
</tbody>
</table>
<h4 id="les-spéciales-">Les spéciales :</h4>
<table>
<thead>
<tr>
<th style="text-align: center;">Symbole</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">++</code></td>
<td>Incrémentation de 1</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">--</code></td>
<td>Décrémentation de 1</td>
</tr>
</tbody>
</table>
<h4 id="les-condensées-">Les condensées :</h4>
<table>
<thead>
<tr>
<th style="text-align: center;">Symbole</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">+=</code></td>
<td>Incrémente la variable de ce qui suit</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">/=</code></td>
<td>divise la variable de ce qui suit</td>
</tr>
</tbody>
</table>
<em>Remarque :</em> L’opérateur <code class="csharp language-csharp">/</code> renvoie une valeur du même type que les nombres utilisés (danger avec des <code class="csharp language-csharp">int</code>)
<h3 id="les-chaines-de-caractère">Les chaines de caractère</h3>
&nbsp;
<table>
<thead>
<tr>
<th style="text-align: center;">Symbole</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">+</code></td>
<td>Accole deux chaînes ensemble</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">\</code></td>
<td>Et non<code class="csharp language-csharp">/</code>, permet l'insertion de caractères spéciaux</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">n</code></td>
<td>Retour à la ligne</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">t</code></td>
<td>Tabulation de la ligne</td>
</tr>
</tbody>
</table>
<h4 id="astuces-">Astuces :</h4>
<ul>
 	<li>On peut utiliser le caractère <code class="csharp language-csharp">\</code> dans un texte en le faisant précéder de lui même</li>
</ul>
<pre><code class="csharp language-csharp">string1 = "Ceci ne s'affichera pas \ ici"
string2 = "Ceci permettra au caractère d'être affiché \\ ici"</code></pre>
<ul>
 	<li>On peut faire précéder la chaîne de caractères par <code class="csharp language-csharp">@</code> pour indiquer que l’on souhaite que ce qui suit reste tel quel</li>
</ul>
<pre><code class="csharp language-csharp">string1 = "Ceci ne s'affichera pas \ ici"
string2 = @"Ceci permettra au caractère d'être affiché \ ici"</code></pre>
<h3 id="opérateurs-de-comparaison">Opérateurs de comparaison</h3>
<h4 id="de-booléens">De booléens</h4>
<table>
<thead>
<tr>
<th style="text-align: center;">Opérateur</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">&amp;&amp;</code></td>
<td>ET logique</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">||</code></td>
<td>OU logique</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">!</code></td>
<td>Négation*</td>
</tr>
</tbody>
</table>
*à combiner avec un autre opérateur : <code class="csharp language-csharp">!&amp;&amp;</code> ou bien <code class="csharp language-csharp">!||</code>
<h4 id="de-nombres">De nombres</h4>
<table>
<thead>
<tr>
<th style="text-align: center;">Opérateur</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">==</code></td>
<td>Egalité</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">!=</code></td>
<td>Différence</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">&gt;</code></td>
<td>Supérieur à</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">&lt;</code></td>
<td>Inférieur à</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">&gt;=</code></td>
<td>Supérieur ou égal</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">&lt;=</code></td>
<td>Inférieur ou égal</td>
</tr>
</tbody>
</table>
<h2 id="les-boucles">Les boucles</h2>
<h3 id="if">If</h3>
Se fait avec l'instruction <code class="csharp language-csharp">if</code>.

Le "sinon" se fait avec <code class="csharp language-csharp">else</code>

On peut faire un "sinon si" avec la combinaison des deux : <code class="csharp language-csharp">else if</code>

Le <code class="csharp language-csharp">if</code> peut aussi vérifier la valeur d'une variable de type booléen

<em>Remarque :</em> Ne nécessite un <code class="csharp language-csharp">;</code> qu'à la fin des instructions pas à la ligne du <code class="csharp language-csharp">if</code>
<pre><code class="csharp language-csharp">bool condition = true;
bool condition2 = true;

if (condition)
{
    Console.WriteLine("La condition est vérifiée.");
}
else if (condition2)
{
    Console.WriteLine("Une des conditions est juste.");
}

else
{
    Console.WriteLine("Les conditions ne sont pas vérifiées.");
}</code></pre>
<h3 id="case">case</h3>
Permet de remplacer un <code class="csharp language-csharp">if</code> s'il y a beaucoup de possibilités

Exécute les instructions jusqu'au <code class="csharp language-csharp">break</code>

Exécute le code après "default" si aucune des conditions n'est remplie

S’utilise avec <code class="csharp language-csharp">:</code>

On peut enchainer plusieurs <code class="csharp language-csharp">case</code> avant l'instruction
<pre><code class="csharp language-csharp">switch (variable)  
{  
    case "cas 1" :  
        // instruction 1;  
        break;  
    case "cas 2":  
    case "cas 3":  
        // instruction pour 2 et 3;  
        break;  
    default:  
        instruction si aucune des conditions n'est remplie;  
        break;  
}</code></pre>
<h3 id="for">For</h3>
Elle est composée de 3 parties : l’initialisation du compteur, la condition de fin et l’incrémentation du compteur.
On met les instructions dans un bloc de code à la suite.
Le compteur est défini dans la boucle
<pre><code class="csharp language-csharp">for (int compteur = 0; compteur &lt; 50; compteur++)  
{  
    Console.WriteLine("Bonjour C#");  
}</code></pre>
<em>Remarques :</em> si on utilise cette boucle pour parcourir un tableau, prendre soin de ne pas dépasser la taille du tableau !
Pour cela on peut utiliser <code class="csharp language-csharp">tableau.Length</code>
<h3 id="foreach">Foreach</h3>
Permet de parcourir un tableau en attribuant à une variable successivement les valeurs des éléments.

Comme cette variable change à chaque itération il n’est <strong>pas possible</strong> de la modifier dans la boucle.
<pre><code class="csharp language-csharp">foreach (string element in tableau)  
{  
    Console.WriteLine(element);  
}  </code></pre>
<em>Remarque :</em> il vaut mieux ne pas modifier la liste que l’on est en train de parcourir !
<h3 id="while">While</h3>
Répète le bloc de code qui suit l’instruction tant que la condition du <code class="csharp language-csharp">while</code> est vraie.
<pre><code class="csharp language-csharp">while (bool condition == True)  
{  
    Instructions;  
}  </code></pre>
<h4 id="alternative">Alternative</h4>
Il est possible de lancer la boucle une première fois avant d’inspecter la condition, on déclare les instructions avec <code class="csharp language-csharp">do</code>

On passera au moins une fois dans le corps de la boucle ici car la condition de sortie de boucle est évaluée à la fin.
<pre><code class="csharp language-csharp">int i = 0;  
do  
{  
    Console.WriteLine("Bonjour C#");  
    i++;  
}  
while (i &lt; 50);  </code></pre>
<h3 id="break-et-continue">Break et continue</h3>
Elles ont un fonctionnement très simple :
<h4 id="break">Break</h4>
L’instruction <code class="csharp language-csharp">break</code> provoque une sortie immédiate de la boucle
<pre><code class="csharp language-csharp">int i = 0;  
while (true)  
{  
    if (i &gt;= 50)  
    {  
        break;  
    }  
    Console.WriteLine("Bonjour C#");  
    i++;  
}</code></pre>
<h4 id="continue">Continue</h4>
L’instruction <code class="csharp language-csharp">continue</code> passe directement à l’itération suivante.
<pre><code class="csharp language-csharp">// Afficher les nombres impairs
for (int i = 0; i &lt; 20; i++)  
{  
    if (i % 2 == 0)  
    {  
        continue;  
    }  
    Console.WriteLine(i);  
}  </code></pre>
<h2 id="les-blocs-de-code">Les blocs de code</h2>
Les blocs de code sont, délimités par des accolades : <code class="csharp language-csharp">{___}</code>

Il est possible de définir des <em>variables locales</em> dans le bloc de code mais il faut se méfier car elles seront <strong>"détruites"</strong> à la fin du bloc de code.
<h2 id="les-méthodes-ou-fonctions">Les "méthodes" ou fonctions</h2>
On doit les définir en dehors de la méthode dans laquelle est exécuté le programme (main).
<h3 id="descripteurs">Descripteurs</h3>
Lorsque l'on les définit, on utilise comme dans le cas des variables des descripteurs :

Lorsque l'on les définit, on utilise comme dans le cas des variables des descripteurs :
<table>
<thead>
<tr>
<th style="text-align: center;">Descripteur</th>
<th>Utilisation</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">void</code></td>
<td>Indique que la méthode ne retourne aucune valeur.</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">static</code></td>
<td>pour utiliser des méthodes dans le main, elles doivent être du même type que la méthode main, soit, statique</td>
</tr>
</tbody>
</table>
<pre><code class="csharp language-csharp">static void nom_de_la_methode(type_du_paramètre paramètre1, int nombre_x)
{
  // instructions;
  // instructions;
}   </code></pre>
<h3 id="valeur-de-retour">Valeur de retour</h3>
On utilise le mot clef <code class="csharp language-csharp">return</code> et au lieu de <code class="csharp language-csharp">void</code>, on indique le type de valeur retournée par la méthode.

Si on indique que la méthode retourne une valeur, il faut impérativement qu'elle le fasse peu importe ce qui est rentré en paramètre, il faut que le logiciel rencontre l'instruction <code class="csharp language-csharp">return</code>.
<pre><code class="csharp language-csharp">static int methode_avec_retour(type_du_paramètre paramètre1, int nombre_x)
{  
  int variable;
  // instructions;
  // instructions;

  return variable;
}  </code></pre>
<h2 id="les-ensembles-de-données">Les ensembles de données</h2>
<h3 id="les-tableaux">Les tableaux</h3>
Les types de données dans un tableau sont définies avec les mêmes noms plus un <code class="csharp language-csharp">[  ]</code> (par exemple : <code class="csharp language-csharp">int[]</code> )

<em>Remarque :</em> Un tableau est de taille fixe
<h4 id="création-dun-tableau">Création d'un tableau</h4>
On utilise l'instruction <code class="csharp language-csharp">new type_du_tableau[5]</code>

On peut atteindre une donnée par son indice <code class="csharp language-csharp">tableau[4]</code> cherchera la 5ème valeur car les indices débutent à 0

<code class="csharp language-csharp">Array.Sort()</code> permet de trier le tableau par valeurs croissantes
<h4 id="syntaxe">Syntaxe</h4>
<pre><code class="csharp language-csharp">string[] tableau = new string[nombre_éléments];
tableau[0] = "1er élément";  
tableau[1] = "2nd élément";
....</code></pre>
Ou bien en plus condensé :
<pre><code class="csharp language-csharp">string[] jours = new string[] { "Lundi", "Mardi", "Mercredi", "Jeudi", "Vendredi", "Samedi", "Dimanche" };</code></pre>
<em>Remarque :</em> un tableau peut être multidimensionnel !
<h3 id="les-listes">Les listes</h3>
Elles fonctionnent comme les tableaux mais possèdent quand même des différences notables.

Le type d'une liste s'écrit avec des <code class="csharp language-csharp">&lt;&gt;</code>.
<h4 id="outils">Outils</h4>
<table>
<thead>
<tr>
<th style="text-align: center;">Nom</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">nom_liste.Add(elt_à_ajouter)</code></td>
<td>Ajouter des éléments à une liste</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">nom_liste.RemoveAt(indice_élément)</code></td>
<td>Enlever un élément</td>
</tr>
<tr>
<td style="text-align: center;"><code class="csharp language-csharp">nom_liste.IndexOf(élément)</code></td>
<td>Donne l'indice d'un élément</td>
</tr>
</tbody>
</table>
Les listes et les tableaux ne peuvent contenir qu’un seul type d’éléments.

Ce sont des types génériques : on a un tableau de <strong>_ ou une liste de _</strong> (string, int…)
<pre><code class="csharp language-csharp">List&lt;string&gt; chaines = new List&lt;string&gt;(); // création de la liste
chaines.Add("chaine"); // compilation OK
chaines.Add(1); // compilation KO, on ne peut pas ajouter un entier dans une liste de chaines de caractères
chaines.Add("1"); // compilation OK, c'est une chaine de caractères</code></pre>
<h3 id="les-énumérations">Les énumérations</h3>
On peut les définir en dehors de la méthode main.

Leur principal intérêt est qu'elles définissent un nouveau type de données dont les valeurs sont limitées et fixées. Exemple, on peut définir un type <code class="csharp language-csharp">joursSemaine</code> ne comprenant que les 7 jours de la semaine.

Il est possible de forcer la valeur d'un élément de l'énumération.

On peut utiliser la syntaxe <code class="csharp language-csharp">Nom.Valeur</code> (par ex : <code class="csharp language-csharp">joursSemaine.Lundi</code>)

Cela peut servir comme une base de donnée.
<pre><code class="csharp language-csharp">enum Nom  
{  
elt_a,  // elt_a vaut 0  
elt_b, // elt_b vaut 1  
elt_c = 5,  // elt_c vaut 5  
elt_d // elt_d vaut 6  
}  </code></pre>
<h2 id="le-framework-net">Le framework .NET</h2>
Pour utiliser certaines fonctionnalités, il est nécessaire d'importer un ensemble de méthodes. On les repère par leur espace de nom (<code class="csharp language-csharp">System</code>, <code class="csharp language-csharp">Console</code>…)

On utilise pour cela l'instruction <code class="csharp language-csharp">using nomLibrairie;</code>

Cela permet entre autres de ne plus avoir à taper le préfixe <code class="csharp language-csharp">Console.</code> par exemple.

On peut accéder aux méthodes incluses dans le framework .NET ici : <a href="http://msdn.microsoft.com/fr-fr/library/.">http://msdn.microsoft.com/fr-fr/library/.</a>

Un fichier .dll est une <code class="csharp language-csharp">assembly</code> = bibliothèque de méthodes. Les bibliothèques appelées sont classées sous le panneau références de l’explorateur de solution
<h2 id="conversion-entre-les-types-de-données">Conversion entre les types de données</h2>
<h3 id="directement">Directement</h3>
On peut demander de stocker dans une variable de type plus large une valeur d’un autre type

<code class="csharp language-csharp">short</code> $rightarrow$ <code class="csharp language-csharp">int</code>

Autrement il nous demandera une conversion explicite !
<h3 id="conversion-explicite">Conversion explicite</h3>
Il faut alors demander au compilateur de traiter la valeur comme le type d’arrivée
<pre><code class="csharp language-csharp">int i = 200;  
short s = (short)i;  </code></pre>
Cela permet de faire sauter les vérifications de type mais cela implique alors aussi des erreurs possibles non détectées.

Il est aussi possible d’obtenir la valeur d’une énumération par ce biais.
<pre><code class="csharp language-csharp">int valeur = (int)Jours.Lundi; // valeur vaut 5</code></pre>
<h3 id="entre-types-incompatibles">Entre types incompatibles</h3>
<code class="csharp language-csharp">str</code> $rightarrow$ <code class="csharp language-csharp">int</code>

D’une chaine de caractères contenant uniquement des chiffres
On utilise <code class="csharp language-csharp">Convert.ToInt32(Variable);</code> ou bien <code class="csharp language-csharp">int.Parse(Variable);</code>.

L’inconvénient est que lorsque la conversion n’est pas possible car l’entrée contient des lettres par exemple, la méthode renvoie une erreur.

Il existe une méthode qui teste la chaine d’entrée et qui la convertit si c’est possible, c’est le cas de <code class="csharp language-csharp">type.TryParse(chaineEntrée, out variableSortie)</code>
<pre><code class="csharp language-csharp">string chaineAge = "ab20cd";  
int age;  
if (int.TryParse(chaineAge, out age))  
{  
    Console.WriteLine("La conversion est possible, age vaut " + age);  
}  
else  
{  
    Console.WriteLine("Conversion impossible");  
}  </code></pre>
<em>Remarque :</em> Les méthodes s’écrivent de manière plus générale <code class="csharp language-csharp">Convert.To|Type|()</code> et <code class="csharp language-csharp">|Type|.TryParse()</code>.
<h2 id="interactions-avec-l’utilisateur">Interactions avec l’utilisateur</h2>
<h3 id="récupérer-un-texte">Récupérer un texte</h3>
Il existe pour cela l’instruction <code class="csharp language-csharp">Console.ReadLine();</code> qui va récupérer sous la forme d’une chaine de caractères tout ce qu’aura saisi l’utilisateur jusqu’à l’appui sur « Entrée »
<pre><code class="csharp language-csharp">// Initialisation  
bool nbrIsValid = false;  
int nbr = -1;  

// Test et conversion  
while (!nbrIsValid)  
{  
    Console.WriteLine("Veuillez saisir un nombre");  
    string saisie = Console.ReadLine();  
    if (int.TryParse(saisie, out nbr))  
        nbrIsValid = true;  
    else  
    {  
        nbrIsValid = false;  
        Console.WriteLine("Le nombre que vous avez saisi est incorrect ...");  
    }  
}  
Console.WriteLine("Votre nombre est le : " + nbr);  </code></pre>
<h3 id="lecture-d’un-caractère">Lecture d’un caractère</h3>
On utilise l’instruction <code class="csharp language-csharp">Console.ReadKey()</code> qui va capturer la première touche saisie au clavier at qui va la renvoyer sous la forme <code class="csharp language-csharp">ConsoleKey.|Touche|</code> utile pour les comparaisons dans une boucle par exemple.

On peut entrer <code class="csharp language-csharp">true</code> en paramètre pour masquer la saisie de l’utilisateur : <code class="csharp language-csharp">Console.ReadKey(true)</code>.
<h2 id="programmation-orientée-objet">Programmation orientée objet</h2>
Il est important de séparer deux notions.
<ul>
 	<li>L’objet en tant que définition de lui-même : descriptions de ses propriétés et de ses actions.</li>
</ul>
<pre><code class="mermaid language-mermaid">graph LR

    style def fill:#C5E1A5,stroke:#8BC34A,stroke-width:2px

    def{&lt;br&gt;&lt;br&gt;Définition&lt;br&gt;&lt;br&gt;&lt;br&gt;}

    subgraph ""
    i1(Propriétés)
    i2(Actions)
    end

    i1 --&gt; def
    i2 --&gt; def</code></pre>
<ul>
 	<li>L’objet en tant qu’instance(s) qui est une entité distincte de l’objet créée à partir de la définition.</li>
</ul>
<pre><code class="mermaid language-mermaid">graph LR

    style i1 fill:#D7CCC8,stroke:#795548,stroke-width:2px
    style i2 fill:#D7CCC8,stroke:#795548,stroke-width:2px
    style i3 fill:#D7CCC8,stroke:#795548,stroke-width:2px
    style i4 fill:#D7CCC8,stroke:#795548,stroke-width:2px
    style i5 fill:#D7CCC8,stroke:#795548,stroke-width:2px
    style def fill:#C5E1A5,stroke:#8BC34A,stroke-width:2px


    def{&lt;br&gt;&lt;br&gt;Définition&lt;br&gt;&lt;br&gt;&lt;br&gt;}

    i1((Instance 1))
    i2((Instance 2))
    i3((Instance 3))
    i4((Instance 4))
    i5((Instance 5))

    i1 --- def
    i2 --- def
    def --- i3
    def --- i4
    def --- i5</code></pre>
<h3 id="encapsulation">Encapsulation</h3>
Tout code (procédures et actions) définies avec l’objet sont protégées. Rien n’est accessible et/ou modifiable de l’extérieur !
<h3 id="héritage">Héritage</h3>
Les objets créés peuvent hériter de certaines (ou de toutes) les caractéristiques. Ainsi l’objet fils aura une partie des propriétés et actions du père mais pourra aussi avoir des spécificités qui lui sont uniques. Plus on remonte dans la hiérarchie, plus les objets sont généraux, plus on descend, plus ils se spécialisent.
Un objet peut avoir plusieurs fils mais un seul père uniquement !
<h3 id="polymorphisme">Polymorphisme</h3>
Un objet peut effectuer la même action avec plusieurs interlocuteurs.
<h3 id="substitution">Substitution</h3>
Un objet qui hérite d’une caractéristique du père peut la modifier avant de se l’approprier.