# Construire un écran de connexion (partie 1)

TP du module 4 – Les bases du CSS

> **Note:** Avant de démarrer ce TP, il convient d’avoir suivi les vidéos des modules 1 à 4 et d’avoir réalisé les TP proposés.

**Durée Estimée : 2h**

## Enonce

Créer un nouveau projet Web.

- Un dossier qui porte par exemple le nom "tp_fil_rouge"
- Dans ce dossier :
    - Creer un fichier **index.html**
    - Creer u nfichier **main.css**

L’objectif est de reproduire cet écran de connexion en HTML/CSS

<p align="center">
  <img src="screenshot_01.png" alt="Screenshot">
</p>

## Etape 1 - La structure

Votre fichier HTML va contenir au moins ces élèments par défaut (vous pouvez copier coller)

```html
<!DOCTYPE html>
<html>

<head>
    <title>La Chocolatine</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
</body>

</html>
```

Placez les éléments importants sans style, tels que :

- Le titre H1 "Connexion au site"
- Un paragraphe qui va contenir le texte d'accueil
- Le champ input **email**
- Le champ input **mot de passe**
- Un lien hypertexte vide pour le **Mot de passe oublié ?**
- Le bouton de connexion
- Le dernier paragraphe restant (S'inscrire sera aussi un lien hypertexte)

> **Note:** Les éléments ne vont pas nécessairement **s'afficher ligne par ligne** pour le moment

Vous devrez avoir un résultat proche de cela :

<p align="center">
  <img src="screenshot_02.png" alt="Screenshot">
</p>

## Etape 2 - Préparation du CSS

> ⚠️ **Important:** Toutes **nos classes css** seront préfixées  de `tp-`

Préparez les **classes CSS** nécessaires pour **aligner les textes au centre** et modifiez la largeur des **champs de saisie et des boutons** afin qu'ils occupent toute la largeur de l'écran.

Ainsi, certains éléments passeront automatiquement à la ligne et vous obtiendrez un résultat similaire à celui-ci

<p align="center">
  <img src="screenshot_03.png" alt="Screenshot">
</p>

## Etape 3 - Finaliser le CSS

Placer une image de fond dans le body graçe à l'attribut **css** `background` ou `background-image`

Utiliser aussi l'attribut `background-size : cover;` essayer d'adapter l'image à la taille de l'écran.

Dans le dossier « ressources » de l'énoncé, vous trouverez l'image de fond

> **Note:** Si l'image n'est pas parfaitement adaptée, ne perdez pas de temps sur ce petit détail. Vous reviendrez dessus une fois tout terminé.

### Quelques astuces/informations 

- Par défaut, les champs de saisie n'auront pas de couleur de fond
- Si vous souhaitez gérer correctement les espacements entre les éléments, je vous conseille **d'encapsuler ces éléments** dans un **div** qui contiendra un **padding**

Exemple de champ encapsulé pour gérer l'espacement **sans margin** d'un champ :

```html
<!-- Champ email -->
<div class="tp-form-block">
    <input class="tp-input" type="text" placeholder="Email">
</div>
```