# [Git] Utiliser Git

Il sert à garder une trace des changements effectués dans les fichiers et les dossiers

## Les Bases

<div>
  <svg version="1.1" id="Calque_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
  	 viewBox="0 0 1024 600" style="enable-background:new 0 0 1024 600;" xml:space="preserve">
  <style type="text/css">
  	.st00{fill:#204056;}
  	.st01{fill:#FFFFFF;}
  	.st02{fill:#BCBEC0;}
  	.st03{font-family:'Consolas';}
  	.st04{font-size:14px;}
  	.st05{font-size:22px;}
  </style>
  <rect id="Fond" y="0" class="st00" width="1025.2" height="600"/>
  <polygon id="Flèche_gauche" class="st01" points="367.8,225.2 367.1,225.9 370.2,228.8 272.2,228.8 272.2,229.8 370.2,229.8
  	367.1,232.7 367.8,233.4 372.2,229.3 "/>
  <polygon id="Flèche_droite" class="st01" points="667.8,225.2 667.1,225.9 670.2,228.8 572.2,228.8 572.2,229.8 670.2,229.8
  	667.1,232.7 667.8,233.4 672.2,229.3 "/>
  <g id="Répertoire_actif">
  	<text transform="matrix(1 0 0 1 143.5 360)"><tspan x="0" y="0" class="st02 st03 st04">Apporter des </tspan><tspan x="0" y="16.8" class="st02 st03 st04">changements aux </tspan><tspan x="0" y="33.6" class="st02 st03 st04">fichiers</tspan><tspan x="0" y="67.2" class="st02 st03 st04">+ ajouts</tspan><tspan x="0" y="84" class="st02 st03 st04">- Suppressions</tspan><tspan x="0" y="100.8" class="st02 st03 st04">~ modifications</tspan></text>
  	<rect id="Ligne_2_" x="143.2" y="328.8" class="st02" width="140" height="1"/>
  	<text transform="matrix(1 0 0 1 143.6665 279.0002)"><tspan x="0" y="0" class="st01 st03 st05">Working</tspan><tspan x="0" y="26.4" class="st01 st03 st05">Directory</tspan></text>
  	<path id="Outils" class="st01" d="M192.2,216.4l2.5-2.5v-4.5l-2.9,2.9h-1.5v-1.5l2.9-2.9h-4.5l-2.5,2.5v3.1l-3.3,3.3l-3-3l1.4-1.4
  		l-1.2-2l0.1-0.1c1.3-1.2,2.2-1.7,3.2-1.4l2.2,0.6l-1.8-1.4c-1.9-1.6-4.6-1.4-6.3,0.3l-4.1,4.1l-0.4,1.7c0,0,0,0,0,0
  		c-0.6-0.2-1.1-0.2-1.5,0.2l0,0l-1.6,1.6l0,0c-0.3,0.3-0.4,0.9-0.2,1.5c0.2,0.6,0.5,1.1,1,1.6c0.7,0.7,1.5,1.1,2.2,1.1
  		c0.3,0,0.6-0.1,0.8-0.3l0,0l0,0c0,0,0,0,0,0c0,0,0,0,0-0.1l1.5-1.5l0,0c0.3-0.4,0.4-0.9,0.2-1.5l1.6-0.3l0.3-0.3l3,3l-2.1,2.1h-3.1
  		l-2.5,2.5v4.6l2.9-2.9h1.5v1.4l-2.9,2.9h4.5l2.5-2.4V224l1.7-1.7l6.9,6.9l3.1-3.1l-6.9-6.8l2.9-2.9H192.2z M172.8,215
  		c0.4,0.2,0.8,0.4,1.2,0.8c0.8,0.8,0.9,1.6,0.8,1.7l0,0l-0.6,0.6c-0.2-0.5-0.5-1-1-1.5c-0.5-0.5-1-0.8-1.5-1l0.7-0.7l0,0
  		C172.4,214.9,172.6,214.9,172.8,215z M173.2,219.1c-0.1,0.1-0.9,0-1.7-0.8c-0.4-0.4-0.7-0.8-0.8-1.2c-0.1-0.3,0-0.5,0-0.5
  		c0,0,0,0,0.1,0l0,0l0,0c0,0,0.1,0,0.1,0c0.3,0,0.9,0.2,1.5,0.8C173.2,218.2,173.3,219,173.2,219.1z M176.9,215.4l-1.6,0.3l-1.2-1.2
  		l0.3-1.6l3.9-3.9c0.9-0.9,2.2-1.2,3.4-1c-0.8,0.3-1.5,0.9-2.1,1.5c-0.1,0.2-0.3,0.3-0.4,0.5l-0.2,0.3l1.1,1.9l-0.8,0.8l-0.1,0
  		l-2.3,2.3V215.4L176.9,215.4z M179.3,214.5l3.6,3.6L182,219l-3.6-3.6L179.3,214.5z M180.4,223.6v3.1l-1.9,1.9h-1.7l1.5-1.4v-2.9
  		l-2.9-0.1l-1.5,1.5V224l1.9-1.9h3.1l2-2l1.5,1.5L180.4,223.6z M190,227.7l-7.6-7.6l1.7-1.7l7.6,7.6L190,227.7z M185.5,218.5
  		L184,217l3.2-3.2v-3.1l1.9-1.9h1.7l-1.5,1.5v2.8l2.9,0.1l1.5-1.5v1.7l-1.9,1.9h-3.1L185.5,218.5z"/>
  	<path id="Dossier" class="st01" d="M220.2,191.8h-59v-2c0-0.6-0.4-1-1-1h-16c-0.6,0-1,0.4-1,2v50c0-0.4,0.4,0,1,0h76
  		c0.6,0,1-0.4,1,0v-47C221.2,192.2,220.8,191.8,220.2,191.8z M220.2,239.8h-76v-43h76V239.8z M220.2,195.8h-76v-6h16v3h60V195.8z"/>
  	<text transform="matrix(0.6595 0 0 1 143.3237 168.9585)" class="st02 st03 st04">1 - Répertoire actif</text>
  </g>
  <g id="Répertoire_de_travail">
  	<text transform="matrix(1 0 0 1 433.5 359)"><tspan x="0" y="0" class="st02 st03 st04">Importer les </tspan><tspan x="0" y="16.8" class="st02 st03 st04">changements dans </tspan><tspan x="0" y="33.6" class="st02 st03 st04">le répertoire de</tspan><tspan x="0" y="50.4" class="st02 st03 st04">travail</tspan></text>
  	<rect id="Ligne_1_" x="433.2" y="328.8" class="st02" width="140" height="1"/>
  	<text transform="matrix(1 0 0 1 433.6665 279.0002)"><tspan x="0" y="0" class="st01 st03 st05">Staging</tspan><tspan x="0" y="26.4" class="st01 st03 st05">Area</tspan></text>
  	<g id="Fichier">
  		<path class="st01" d="M481.2,207h-18h-1v1v19.5v1h1h18h1v-1V208v-1H481.2z M481.2,227.5h-18V208h18V227.5z"/>
  		<rect x="466.2" y="212.8" class="st01" width="1.5" height="1"/>
  		<rect x="469.2" y="212.8" class="st01" width="9" height="1"/>
  		<rect x="466.2" y="215.8" class="st01" width="1.5" height="1"/>
  		<rect x="469.2" y="215.8" class="st01" width="9" height="1"/>
  		<rect x="466.2" y="218.8" class="st01" width="1.5" height="1"/>
  		<rect x="469.2" y="218.8" class="st01" width="9" height="1"/>
  		<rect x="466.2" y="221.8" class="st01" width="1.5" height="1"/>
  		<rect x="469.2" y="221.8" class="st01" width="9" height="1"/>
  	</g>
  	<path id="Dossier_1_" class="st01" d="M510.2,191.8h-59v-2c0-0.6-0.4-1-1-1h-16c-0.6,0-1,0.4-1,2v50c0-0.4,0.4,0,1,0h76
  		c0.6,0,1-0.4,1,0v-47C511.2,192.2,510.8,191.8,510.2,191.8z M510.2,239.8h-76v-43h76V239.8z M510.2,195.8h-76v-6h16v3h60V195.8z"/>
  	<text transform="matrix(0.6595 0 0 1 433.8237 169.0835)" class="st02 st03 st04">2 - Répertoire de travail</text>
  </g>
  <g id="Répertoire_Git">
  	<text transform="matrix(1 0 0 1 743 359)"><tspan x="0" y="0" class="st02 st03 st04">Enregistrer les</tspan><tspan x="0" y="16.8" class="st02 st03 st04">changements dans</tspan><tspan x="0" y="33.6" class="st02 st03 st04">le répertoire Git</tspan><tspan x="0" y="50.4" class="st02 st03 st04">en tant que nouvel</tspan><tspan x="0" y="67.2" class="st02 st03 st04">‘amendement’</tspan></text>
  	<rect id="Ligne" x="743.2" y="328.8" class="st02" width="140" height="1"/>
  	<text transform="matrix(1 0 0 1 744.1665 279.0002)" class="st01 st03 st05">Repository</text>
  	<path id="BDD" class="st01" d="M792.4,220.5v-4c0.1-0.2,0.2-0.4,0.2-0.6c0-0.3-0.1-0.6-0.4-0.8c0.1-0.2,0.2-0.4,0.2-0.6V210
  		c0-2.6-7.8-2.8-10.2-2.8S772,207.4,772,210v4.5c0,0.3,0.1,0.6,0.3,0.8c-0.2,0.2-0.3,0.4-0.3,0.7v4.5c0,0.3,0.1,0.6,0.3,0.8
  		c-0.2,0.2-0.3,0.4-0.3,0.7v4.5c0,2.6,7.8,2.8,10.2,2.8c2.4,0,10.2-0.2,10.2-2.8V222l0,0c0-0.3-0.1-0.5-0.3-0.7
  		C792.3,221,792.4,220.8,792.4,220.5z M773.1,216c2.2,1.2,7.2,1.3,9.1,1.3c1.9,0,7.2-0.1,9.3-1.5c0.1,0.1,0.1,0.1,0.1,0.1
  		c0,0,0,0.1,0,0.1h-0.2v0.2c-0.7,0.6-3.1,1.5-9,1.5C775.3,217.7,773.1,216.5,773.1,216C773.1,216,773.1,216,773.1,216z M782.2,208.3
  		c7.1,0,9.2,1.3,9.2,1.8s-2.2,1.8-9.2,1.8s-9.2-1.3-9.2-1.8S775.1,208.3,782.2,208.3z M773,214.5v-3.1c2.2,1.3,7.3,1.4,9.2,1.4
  		s7-0.1,9.2-1.4v3.1c0,0.5-2.2,1.8-9.2,1.8c-6.1,0-8.6-1-9.1-1.6l0,0c0,0,0,0,0,0C773,214.6,773,214.6,773,214.5z M773,220.5v-3.1
  		c2.2,1.3,7.3,1.4,9.2,1.4c1.8,0,6.9-0.1,9.2-1.4v3.1c0,0.5-2.2,1.8-9.2,1.8c-6.1,0-8.6-1-9.1-1.6l0,0c0,0,0,0,0,0
  		C773,220.6,773,220.6,773,220.5z M782.2,228.3c-7,0-9.2-1.3-9.2-1.8v-3.1c2.2,1.3,7.3,1.4,9.2,1.4s7-0.1,9.2-1.4v3.1
  		C791.4,227,789.2,228.3,782.2,228.3z M791.4,222v0.1c-0.5,0.6-2.9,1.6-9.1,1.6c-7.1,0-9.3-1.2-9.3-1.7c0,0,0,0,0-0.1
  		c2.2,1.3,7.3,1.4,9.2,1.4c1.9,0,7.1-0.1,9.3-1.5C791.5,221.9,791.5,221.9,791.4,222C791.5,221.9,791.5,222,791.4,222L791.4,222z"/>
  	<path id="Dossier_2_" class="st01" d="M820.2,191.8h-59v-2c0-0.6-0.4-1-1-1h-16c-0.6,0-1,0.4-1,2v50c0-0.4,0.4,0,1,0h76
  		c0.6,0,1-0.4,1,0v-47C821.2,192.2,820.8,191.8,820.2,191.8z M820.2,239.8h-76v-43h76V239.8z M820.2,195.8h-76v-6h16v3h60V195.8z"/>
  	<text transform="matrix(0.6595 0 0 1 745.3237 169.1585)" class="st02 st03 st04">3 - Répertoire Git</text>
  </g>
  </svg>
</div>

### Créer un répertoire

```git
git init
```

Créé un nouveau répertoire git (`repository`)

Résultat :

```git
Initalized an empty git repository in /home/ccuser/workspace/sorcerers-code/.git/
```

---

### Obtenir le statut

```git
git status
```

Inspecte le contenu du répertoire actif (`working`) et le répertoire de travail (`staging`)

---

### Ajouter des fichiers

```git
git add
```

Ajoute des fichiers du répertoire actif vers le répertoire de travail.

---

### Comparer des répertoires

```git
git diff
```

Compare les deux répertoires (actif et de travail)

Résultat :
```git
diff --git a/index.html b/index.htmlindex c5e1812..12da64d 100644
--- a/index.html
+++ b/index.html@@ -7,6 +7,6 @@
   </head>
   <body>
     <h1 class="title">Welcome to Progate</h1>
-    <p>Learn programming online with Progate!</p>
+    <p class="subtitle">Learn programming online with Progate!</p>
   </body>
 </html>
diff --git a/stylesheet.css b/stylesheet.css
index 1b8e33c..8ff89b3 100644
--- a/stylesheet.css
+++ b/stylesheet.css
@@ -1,3 +1,6 @@
 .title {
   color: #44dcc0;
 }
+.subtitle {
+  color: #8491a5;
+}
```

---

### Enregistrer des modifications

```git
git commit
```

Enregistre de manière permanente les modifications du répertoire de travail

Chaque amendement (`commit`) est enregistré dans le `log`.
On peut utiliser l’attribut `–m` pour inclure un message avec.

### Observer l'arbre de travail
Cela se fait via la commande
```git
git log
```

---

## Défaire des changements

<div>
  <svg version="1.1" id="Calque_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
  	 viewBox="0 0 836 648" style="enable-background:new 0 0 836 648;" xml:space="preserve">
  <style type="text/css">
  	.st20{fill:#204056;}
  	.st21{fill:#52B1DB;}
  	.st22{font-family:'Consolas';}
  	.st23{font-size:18px;}
  	.st24{fill:none;stroke:#FFFFFF;stroke-miterlimit:10;}
  	.st25{opacity:0.25;fill:#FFFFFF;enable-background:new    ;}
  	.st26{fill:#FFFFFF;}
  	.st27{font-size:15px;}
  	.st28{font-size:20px;}
  </style>
  <rect id="Fond" class="st20" width="836" height="648"/>
  <g id="Après">
  	<text transform="matrix(1 0 0 1 399.807 504.2)" class="st21 st22 st23">HEAD</text>
  	<line id="ligne" class="st24" x1="178" y1="474.5" x2="418" y2="474.5"/>
  	<circle id="i5" class="st25" cx="658" cy="474.5" r="8"/>
  	<circle id="i4_1_" class="st25" cx="538" cy="474.5" r="8"/>
  	<circle id="i3_1_" class="st21" cx="418" cy="474.5" r="8"/>
  	<circle id="i2" class="st26" cx="298" cy="474.5" r="8"/>
  	<circle id="i1" class="st26" cx="178" cy="474.5" r="8"/>
  	<text transform="matrix(1 0 0 1 293.877 505.5)" class="st26 st22 st27">b</text>
  	<text transform="matrix(1 0 0 1 173.577 504.9)" class="st26 st22 st27">a</text>
  	<text transform="matrix(1 0 0 1 359.6215 404.8)" class="st26 st22 st28">Après Reset</text>
  </g>
  <g id="Avant">
  	<text transform="matrix(1 0 0 1 533.377 225.6)" class="st26 st22 st27">d</text>
  	<text transform="matrix(1 0 0 1 413.9769 225)" class="st26 st22 st27">c</text>
  	<text transform="matrix(1 0 0 1 294.077 225.8)" class="st26 st22 st27">b</text>
  	<text transform="matrix(1 0 0 1 174.377 223.6)" class="st26 st22 st27">a</text>
  	<text transform="matrix(1 0 0 1 637.207 223)" class="st21 st22 st23">HEAD</text>
  	<line id="ligne_1_" class="st24" x1="178" y1="194.5" x2="658" y2="194.5"/>
  	<circle id="i5_1_" class="st21" cx="658" cy="194.5" r="8"/>
  	<circle id="i4" class="st26" cx="538" cy="194.5" r="8"/>
  	<circle id="i3" class="st26" cx="418" cy="194.5" r="8"/>
  	<circle id="i2_1_" class="st26" cx="298" cy="194.5" r="8"/>
  	<circle id="i1_1_" class="st26" cx="178" cy="194.5" r="8"/>
  	<text transform="matrix(1 0 0 1 359.6215 133.7001)" class="st26 st22 st28">Avant Reset</text>
  </g>
  <g id="Flèche">
  	<line id="trait" class="st24" x1="418.5" y1="294.5" x2="418.5" y2="333.4"/>
  	<polygon id="pointe" class="st26" points="414.4,330.1 415.1,329.4 418.5,333 421.9,329.4 422.6,330.1 418.5,334.5 	"/>
  </g>
  </svg>
</div>

### Depuis le dernier enregistrement

```git
git checkout HEAD filename
```

Retire les changements du répertoire actif depuis le dernier amendement

---

### Pour un fichier en particulier

```git
git reset HEAD filename
```

Retire toute modification du répertoire de travail du fichier en question; il redevient exactement comme lors du dernier amendement

---

### Pour un amendement particulier

```git
git reset SHA
```

Permet de revenir directement à un amendement en particulier. Il faut rentrer les 7 premiers caractères du code SHA

## Créer des branches de modifications
La branche principale est appelée `master`

<div>
  <svg version="1.1" id="CONTENT" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
   viewBox="0 0 836 648" style="enable-background:new 0 0 836 648;" xml:space="preserve">
  <style type="text/css">
  .st10{fill:#204056;}
  .st11{fill:#52B1DB;}
  .st12{fill:none;stroke:#52B1DB;stroke-miterlimit:10;}
  .st13{font-family:'Consolas';}
  .st14{font-size:18px;}
  .st15{fill:#FFFFFF;}
  .st16{fill:none;stroke:#FFFFFF;stroke-miterlimit:10;}
  .st17{font-size:20px;}
  </style>
  <rect id="Fond" class="st10" width="836" height="648"/>
  <g id="Branche">
  <circle id="C42" class="st11" cx="718" cy="294.5" r="8"/>
  <circle id="C41" class="st11" cx="598" cy="294.5" r="8"/>
  <line id="Ligne_B2" class="st12" x1="598" y1="294.5" x2="718" y2="294.5"/>
  <line id="Ligne_B1" class="st12" x1="478" y1="394.5" x2="598" y2="294.5"/>
  <text id="Teste_branche" transform="matrix(1 0 0 1 640.8281 279)" class="st11 st13 st14">Nouvelle Branche</text>
  </g>
  <g id="Master">
  <circle id="C5" class="st15" cx="598" cy="394.5" r="8"/>
  <circle id="C4" class="st15" cx="478" cy="394.5" r="8"/>
  <circle id="C3" class="st15" cx="358" cy="394.5" r="8"/>
  <circle id="C2" class="st15" cx="238" cy="394.5" r="8"/>
  <circle id="C1" class="st15" cx="118" cy="394.5" r="8"/>
  <line id="Ligne" class="st16" x1="118" y1="394.5" x2="598" y2="394.5"/>
  <text id="Texte_master" transform="matrix(1 0 0 1 569.3105 425)" class="st15 st13 st14">Master</text>
  </g>
  <text id="Titre" transform="matrix(1 0 0 1 352.0234 65)" class="st15 st13 st17">Branches Git</text>
  </svg>
</div>

### Obtenir la branche actuelle

```git
git branch
```

Permet de savoir sur quelle branche on se trouve, La commande en donne une liste.

**Résultat :**
```git
$ git branch                                                                                                                                                     
* master
```

---

### Créer une branche

```git
git branch branch_name
```

Créé une nouvelle branche

---

### Changer de branche

```git
git checkout BRANCH_NAME
```

Permet de permuter les branches

**Résultat :**
```git
$ git checkout fencing
Switched to branch 'fencing'
$ git branch
* fencing
  master
```

---

### Fusion de branches

```git
git merge branch_name
```

Permet de fusionner les modifications entre les branches

Si les deux branches modifient la même ligne, un conflit est mis en évidence par git

```git
CONFLICT (content): Merge conflict in resumé.txt
Automatic merge failed; fix conflicts and then commit the result.
```

Dans le fichier :

```git
<<<<<<< HEAD
master version of line
=======
fencing version of line
>>>>>>> fencing
```


---

### Supprimer une branche


```git
git branch -d branch_name
```

Supprime une branche s’il n‘est plus utile de la garder.


## La collaboration avec Git

### Connecter un service de partage de code
on utilise la commande :
```git
git remote add remote_name http://remote.url
```

### Rapatrier les modifications en local

```git
git clone
```

Créé une copie locale du dossier distant

---

### Lister les dossiers distants associés

```git
git remote -v
```

Donne une liste des dossiers distants associés à un projet

---

### Va chercher la dernière version en ligne

```git
git fetch
```

Va chercher la dernière version sur le dossier distant

---

### Fusion de dossiers

```git
git merge origin/master
```

Fusionne le dossier `origin/master` dans le dossier local

---

### Téléverser les modifications

```git
git push remote_name <branch_name>
```

Ajoute la branche au répertoire actif distant

**Résultat :**

```git
To /home/ccuser/workspace/curriculum/science-quizzes
 * [new branch]      bio-questions -> bio-questions
```
