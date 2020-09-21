---
ID: 24
post_title: '[Markdown] Les bases de Markdown'
post_name: les-bases-de-markdown
author: Alexandre
post_date: 2018-02-04 15:30:45
layout: post
link: >
  http://sobieski.name/informatique/markdown/les-bases-de-markdown/
published: true
tags: [ ]
categories:
  - Markdown
---
<p>Une introduction au language <a href="https://guides.github.com/features/mastering-markdown/">Markdown par Github</a>.     </p>
<h2>Markdown ?</h2>
<p><code>Markdown</code> est une manière plus simple de stocker de l'information à l'état pur sur le web. C'est tout simplement un fichier texte avec un formattage particulier. Les options sont nombreuses : formattage en <strong>gras</strong> ou en <em>italique</em>, ajouter des images, créer des listes et des tableaux... Les possibilités sont très nombreuses ! Finalement, Markdown n'est qu'un fichier textuel avec des carractères particuliers comme <code>#</code> ou <code>*</code>.</p>
<h2>Syntaxe</h2>
<h3>Titres</h3>
<pre><code class="language-markdown"># Ceci est un titre &lt;h1&gt;
## Ceci est un titre &lt;h2&gt;
### Ceci est un titre &lt;h3&gt;
#### Ceci est un titre &lt;h4&gt;
##### Ceci est un titre &lt;h5&gt;
###### Ceci est un titre &lt;h6&gt;</code></pre>
<p>Les voici en action :</p>
<hr />
<h1>Ceci est un titre  <h1></h1>
<h2>Ceci est un titre <h2></h2>
<h3>Ceci est un titre <h3></h3>
<h4>Ceci est un titre <h4></h4>
<h5>Ceci est un titre <h5></h5>
<h6>Ceci est un titre <h6></h6>
<hr />
<p><strong><em>Remarque :</em></strong> Pour ajouter un <code>id</code> et/ou une <code>class</code> à un titre, il suffit d'ajouter <code>{#id .class1 .class2}</code>. Par exemple:  </p>
<pre><code class="language-markdown"># Ce titre possède un id      {#my_id}
# Ce titre possède deux classes {.class1 .class2}</code></pre>
<blockquote>
<p>Pas certain que tous les éditeurs l'acceptent.</p>
</blockquote>
<h3>Mettre du texte en avant</h3>
<pre><code class="language-markdown">*Italique*
_Italique aussi_

**Gras**
__Gras aussi__

_Les **effets** sont cumulables_

~~Du texte barré~~</code></pre>
<p>Exemples :</p>
<hr />
<p><em>Italique</em></p>
<p><em>Italique aussi</em></p>
<p><strong>Gras</strong></p>
<p><strong>Gras aussi</strong></p>
<p><em>Les <strong>effets</strong> sont cumulables</em></p>
<p><del>Du texte barré</del></p>
<hr />
<h3>Listes</h3>
<h4>Liste non ordonnée</h4>
<pre><code class="language-markdown">* Item 1
* Item 2
  * Item 2a
  * Item 2b</code></pre>
<ul>
<li>Item 1</li>
<li>Item 2
<ul>
<li>Item 2a</li>
<li>Item 2b</li>
</ul></li>
</ul>
<h4>Liste ordonnée</h4>
<pre><code class="language-markdown">1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b</code></pre>
<ol>
<li>Item 1</li>
<li>Item 2</li>
<li>Item 3
<ol>
<li>Item 3a</li>
<li>Item 3b</li>
</ol></li>
</ol>
<h3>Images</h3>
<pre><code class="language-markdown">![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)</code></pre>
<h3>Liens</h3>
<pre><code class="language-markdown">http://github.com - automatique!
[GitHub](http://github.com)</code></pre>
<p>http://github.com - automatique!</p>
<p><a href="http://github.com">GitHub</a></p>
<h3>Citation</h3>
<pre><code class="language-markdown">Kain West a dit:
&gt; We're living the future so
&gt; the present is our past.
</code></pre>
<p>Kain West a dit:</p>
<blockquote>
<p>We're living the future so
the present is our past.</p>
</blockquote>
<h3>Barre horizontale</h3>
<pre><code class="language-markdown">Trois ou plus...

---

Tirets

***

Asterisques

___

Carractères de soulignement</code></pre>
<h3>Code dans la ligne</h3>
<pre><code class="language-markdown">Je pense que vous devriez utiliser l'élément
`&lt;addr&gt;` ici.</code></pre>
<p>Je pense que vous devriez utiliser l'élément <code>&lt;addr&gt;</code> ici.</p>
<h3>Bloc de code délimité</h3>
<p>Il est possible de créer des blocs de code délimités en plaçant les symboles suivants <code>```</code> avant et après le bloc de code.</p>
<h4>Surlignage syntaxique</h4>
<p>Il est possible de mettre en évidence le code d'un language particulier par le surlignage syntaxique.</p>
<p>Pour par exemple mettre en évidence le code du language <code>Ruby</code> :</p>
<pre><code>```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```</code></pre>
<pre><code class="language-ruby">require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html</code></pre>
<h4>Code block class (MPE extended feature)</h4>
<p>You can set <code>class</code> for your code blocks.  </p>
<p>For example, to add <code>class1 class2</code> to a code block  </p>
<pre><code>```javascript {.class1 .class}
function add(x, y) {
  return x + y
}
```</code></pre>
<h5>line-numbers</h5>
<p>You can enable line number for a code block by adding <code>line-numbers</code> class.  </p>
<p>For example:    </p>
<pre><code>```javascript {.line-numbers}
function add(x, y) {
  return x + y
}
```</code></pre>
<p><img src="https://user-images.githubusercontent.com/1908863/28200587-a8582b0a-6832-11e7-83a7-6c3bb011322f.png" alt="screen shot 2017-07-14 at 1 20 27 am" /></p>
<h3>Task lists</h3>
<pre><code class="language-markdown">- [x] @mentions, #refs, [links](), **formatting**, and &lt;del&gt;tags&lt;/del&gt; supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item</code></pre>
<h3>Tables</h3>
<p>You can create tables by assembling a list of words and dividing them with hyphens <code>-</code> (for the first row), and then separating each column with a pipe <code>|</code>:  </p>
<pre><code class="language-markdown">First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column</code></pre>
<h2>Extended syntax</h2>
<h3>Table</h3>
<p><img src="https://user-images.githubusercontent.com/1908863/28243710-945e3004-699a-11e7-9a5f-d74f6c944c3b.png" alt="screen shot 2017-07-15 at 8 16 45 pm" /></p>
<h3>Emoji &amp; Font-Awesome</h3>
<blockquote>
<p>This only works for <code>markdown-it parser</code> but not <code>pandoc parser</code>.<br />
Enabled by default. You can disable it from the package settings.  </p>
</blockquote>
<pre><code>:smile:
:fa-car:</code></pre>
<h3>Superscript</h3>
<pre><code class="language-markdown">30^th^</code></pre>
<h3>Subscript</h3>
<pre><code class="language-markdown">H~2~O</code></pre>
<h3>Footnotes</h3>
<pre><code class="language-markdown">Content [^1]

[^1]: Hi! This is a footnote</code></pre>
<h3>Abbreviation</h3>
<pre><code class="language-markdown">*[HTML]: Hyper Text Markup Language
*[W3C]:  World Wide Web Consortium
The HTML specification
is maintained by the W3C.</code></pre>
<h3>Mark</h3>
<pre><code class="language-markdown">==marked==</code></pre>
<h3>CriticMarkup</h3>
<p>CriticMarkup is <strong>disabled</strong> by default, but you can enable it from the package settings.<br />
For more information about CriticMarkup, check <a href="http://criticmarkup.com/users-guide.php">CriticMarkup User's Guide</a>.    </p>
<p>There are five types of Critic marks:</p>
<ul>
<li>Addition <code>{++ ++}</code></li>
<li>Deletion <code>{-- --}</code></li>
<li>Substitution <code>{~~ ~&gt; ~~}</code></li>
<li>Comment <code>{&gt;&gt; &lt;&lt;}</code></li>
<li>Highlight <code>{== ==}{&gt;&gt; &lt;&lt;}</code></li>
</ul>
<blockquote>
<p>CriticMarkup only works with the markdown-it parser, but not the pandoc parser.  </p>
</blockquote>
<h2>References</h2>
<ul>
<li><a href="https://guides.github.com/features/mastering-markdown/">Mastering Markdown</a></li>
<li><a href="https://daringfireball.net/projects/markdown/basics">Daring Fireball: Markdown Basics</a></li>
</ul>
<p><a href="math.md">➔ Math</a>
no matches</p>