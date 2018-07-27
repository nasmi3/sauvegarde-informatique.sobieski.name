---
ID: 22
post_title: '[Markdown] Appliquer une classe à un element markdown'
author: Alexandre
post_excerpt: ""
layout: post
permalink: >
  http://sobieski.name/informatique/markdown/appliquer-une-classe-a-un-element-markdown/
published: true
post_date: 2018-02-01 02:22:49
tags: [ ]
categories:
  - Markdown
---
Voici comment appliquer une classe à un élément <code>markdown</code>. A l'image des éléments HTML5, il est possible de mettre une classe en markdown. Cela permet entre autres de modifier la mise en forme de l'élément tout en gardant la syntaxe markdown ce qui n'est pas possible au sein d'une balise HTML.

La syntaxe est la suivante :
<pre><code>![Picture][/pic.jpg]{: class=callout }</code></pre>
ou plus simplement
<pre><code>![Picture][/pic.jpg]{: .callout }</code></pre>