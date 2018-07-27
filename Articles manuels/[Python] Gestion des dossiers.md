# [Python] Gestion des dossiers et des fichiers

## Créer un répertoire s'il n'existe pas

```python
def ensure_dir(file_path):
    directory = os.path.dirname(file_path)
    if not os.path.exists(directory):
        os.makedirs(directory)
```
## Déplacer un fichier

Ce bout de code est à utiliser avec le précédent pour s'assurer de l'absence d'erreurs lors du déplacement !

```python
os.rename("path/to/current/file.foo", "path/to/new/desination/for/file.foo")
```
