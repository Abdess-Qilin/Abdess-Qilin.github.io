# Passionnément - HTML

## :dart: Le but de cet atelier

Transposer le Markdown vers le HTML.

## :one: étape 1 : Préparer l'espace de travail
***
1. Ouvrir le projet avec vscode
2. Ouvrir le terminal dans vscode
3. Faire un `git branch` pour vous assurer que vous êtes bien sur la branche `main`
   - Si vous n'êtes **pas** sur `main`, changez de branche en exécutant la commande:

```
git checkout main
```

5. Créer une nouvelle branche et se positionner dessus en exécutant la commande:

```
git checkout -b version_html
```

6. Modifier toutes les extensions `.md` de votre projet (SAUF README.md) en `.html` (incluant les fichiers .md dans les sous-dossiers des passions)

## :two: étape 2 : Adapter le contenu md en html

On a à présent tous les fichiers HTML dont on a besoin pour notre projet.

Cependant, le contenu est toujours formaté en markdown ! Il faut que l'on corrige ça.

1. Dans chaque fichier html, ajouter le `doctype`, les `balises html`, le `head` et le `title`.
2. Dans chaque fichier, s'aider de [la documentation](https://kourou.oclock.io/?post_type=objectif&p=53373) pour transposer le contenu markdown en HTML .
- Utiliser les balises suivantes pour adapter le contenu des fichiers (sans toucher aux images et aux liens pour le moment):
   - Balises de titre `h1`, `h2`, `h3`...,
   - Balises de paragraphes `p`,
   - Balises d'importance et d'emphase `strong`, `em`,
   - Balises de liste `ul`, `li`, `ol`.

3. Tester le résultat sur le navigateur.

## :three: étape 3 : Push la nouvelle branche

Le contenu étant à présent en HTML, on veut pouvoir l'envoyer sur Github.

1. Vérifier la liste des fichiers modifiés grâce à la commande:

```
git status
```

2. Ajouter tous les fichiers modifiés à la liste des éléments à conserver avec:

```
git add .
```

*Note: Il est également possible d'envoyer chaque fichier un à un grâce à la commande `git add [nom_fichier]` (où on remplacera [nom_fichier] par le nom du fichier)*

3. Enregistrer la modification actuelle comme nouvelle version de notre code grâce à:

```
git commit -m "Version HTML sans liens ni images"
```


4. Envoyer la nouvelle version sur Github grâce à:

```
git push origin version_html
```

## BONUS

Rappel : le bonus demande des connaissances que nous n'avons pas vu encore. Il sera nécessaire d'effectuer des recherches pour le réussir.

1. Vous pouvez maintenant faire en sorte d'afficher l'image correspondant au projet, grâce à la balise HTML dédiée.

2. Vous pouvez aussi ajouter les liens vers chacune des pages-projet dans `index.html`
