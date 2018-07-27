# [Python] Utiliser des variables dans des strings

La syntaxe est relativement simple :

Il faut tout d'abord déclarer le nom des variables avant (au sein de la fonction par exemple)

Ensuite, il suffit d'appliquer la syntaxe suivante :

Remarque : fonctionne uniquement avec $python \leq 3.6$
```python
Nom = "Félix"
age = 30
# Ne pas oublier le "f" avant le début du texte
ligne_de_texte = f"Mon ami {Nom} a {age} ans."
print(ligne_de_texte)
```
> Mon ami Félix a 30 ans.
