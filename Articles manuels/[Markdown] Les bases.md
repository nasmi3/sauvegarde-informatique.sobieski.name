# Les bases de Markdown
Une introduction au language [Markdown par Github](https://guides.github.com/features/mastering-markdown/).     

## Markdown ?  
`Markdown` est une manière plus simple de stocker de l'information à l'état pur sur le web. C'est tout simplement un fichier texte avec un formattage particulier. Les options sont nombreuses : formattage en **gras** ou en *italique*, ajouter des images, créer des listes et des tableaux... Les possibilités sont très nombreuses ! Finalement, Markdown n'est qu'un fichier textuel avec des carractères particuliers comme `#` ou `*`.

## Syntaxe

### Titres
```markdown
# Ceci est un titre <h1>
## Ceci est un titre <h2>
### Ceci est un titre <h3>
#### Ceci est un titre <h4>
##### Ceci est un titre <h5>
###### Ceci est un titre <h6>
```

Les voici en action :

---
# Ceci est un titre  \<h1>
## Ceci est un titre \<h2>
### Ceci est un titre \<h3>
#### Ceci est un titre \<h4>
##### Ceci est un titre \<h5>
###### Ceci est un titre \<h6>
---

***Remarque :*** Pour ajouter un `id` et/ou une `class` à un titre, il suffit d'ajouter `{#id .class1 .class2}`. Par exemple:  
```markdown
# Ce titre possède un id      {#my_id}
# Ce titre possède deux classes {.class1 .class2}
```
> Pas certain que tous les éditeurs l'acceptent.

### Mettre du texte en avant
```markdown
*Italique*
_Italique aussi_

**Gras**
__Gras aussi__

_Les **effets** sont cumulables_

~~Du texte barré~~
```

Exemples :

---
*Italique*

_Italique aussi_

**Gras**

__Gras aussi__

_Les **effets** sont cumulables_

~~Du texte barré~~

---
### Listes
#### Liste non ordonnée
```markdown
* Item 1
* Item 2
  * Item 2a
  * Item 2b
```

* Item 1
* Item 2
  * Item 2a
  * Item 2b

#### Liste ordonnée
```markdown
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b
```

1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b

### Images  
```markdown
![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)
```

### Liens  
```markdown
http://github.com - automatique!
[GitHub](http://github.com)
```
http://github.com - automatique!

[GitHub](http://github.com)

### Citation
```markdown
Kain West a dit:
> We're living the future so
> the present is our past.

```

Kain West a dit:

> We're living the future so
> the present is our past.

### Barre horizontale
```markdown
Trois ou plus...

---

Tirets

***

Asterisques

___

Carractères de soulignement
```

### Code dans la ligne
```markdown  
Je pense que vous devriez utiliser l'élément
`<addr>` ici.
```

Je pense que vous devriez utiliser l'élément `<addr>` ici.

### Bloc de code délimité
Il est possible de créer des blocs de code délimités en plaçant les symboles suivants <code>\`\`\`</code> avant et après le bloc de code.

#### Surlignage syntaxique
Il est possible de mettre en évidence le code d'un language particulier par le surlignage syntaxique.

Pour par exemple mettre en évidence le code du language `Ruby` :

    ```ruby
    require 'redcarpet'
    markdown = Redcarpet.new("Hello World!")
    puts markdown.to_html
    ```

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

#### Code block class (MPE extended feature)
You can set `class` for your code blocks.  

For example, to add `class1 class2` to a code block  

    ```javascript {.class1 .class}
    function add(x, y) {
      return x + y
    }
    ```

##### line-numbers
You can enable line number for a code block by adding `line-numbers` class.  

For example:    

    ```javascript {.line-numbers}
    function add(x, y) {
      return x + y
    }
    ```

![screen shot 2017-07-14 at 1 20 27 am](https://user-images.githubusercontent.com/1908863/28200587-a8582b0a-6832-11e7-83a7-6c3bb011322f.png)


### Task lists   
```markdown  
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
```

### Tables
You can create tables by assembling a list of words and dividing them with hyphens `-` (for the first row), and then separating each column with a pipe `|`:  
```markdown  
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
```


## Extended syntax
### Table  
![screen shot 2017-07-15 at 8 16 45 pm](https://user-images.githubusercontent.com/1908863/28243710-945e3004-699a-11e7-9a5f-d74f6c944c3b.png)

### Emoji & Font-Awesome

> This only works for `markdown-it parser` but not `pandoc parser`.  
> Enabled by default. You can disable it from the package settings.  

```
:smile:
:fa-car:
```

### Superscript
```markdown
30^th^
```

### Subscript
```markdown
H~2~O
```

### Footnotes
```markdown
Content [^1]

[^1]: Hi! This is a footnote
```

### Abbreviation  
```markdown  
*[HTML]: Hyper Text Markup Language
*[W3C]:  World Wide Web Consortium
The HTML specification
is maintained by the W3C.
```

### Mark  
```markdown
==marked==
```

### CriticMarkup  
CriticMarkup is **disabled** by default, but you can enable it from the package settings.    
For more information about CriticMarkup, check [CriticMarkup User's Guide](http://criticmarkup.com/users-guide.php).    

There are five types of Critic marks:

* Addition `{++ ++}`
* Deletion `{-- --}`
* Substitution `{~~ ~> ~~}`
* Comment `{>> <<}`
* Highlight `{== ==}{>> <<}`

> CriticMarkup only works with the markdown-it parser, but not the pandoc parser.  

## References
* [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
* [Daring Fireball: Markdown Basics](https://daringfireball.net/projects/markdown/basics)


[➔ Math](math.md)
no matches
