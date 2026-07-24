---
title: HTML - Chapitre 2 | What's in your <head> ?
description: HTML - Chapitre 2 | What's in your <head> ?
show_toc: true
---

## Objectifs

* Utiliser au mieux la balise head.
* Comprendre à quoi servent les métadonnées.

## Pré-requis

````stepper
# Valider la ressource suivante
[Voir la ressource "HTML - Chapitre 1 | Introduction au HTML"](https://github.com/simplonco/dev-web-html-chapitre-1-introduction-au-html/)
# Connaitre la structure de base d'un document HTML
```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>My super website</title>
</head>
<body>
    <p>Hello World</p>
</body>
</html>
```
````

## Introduction

Précédemment, tu as vu les principes de bases du langage HTML.

La balise `<head>` est la première partie d'un document : c'est la partie de la page qui n'est pas "visible". Pourtant la balise `<head>` contient de nombreuses métadonnées qui sont très utiles au navigateur pour comprendre le contexte d'une page web.

## Dans la tête ?

La balise `<head>` contiens des **informations utiles** à notre **navigateur**.

Elle est située au début de notre document dans la balise `<html>` et avant la balise `<body>`.

```html
<!DOCTYPE html>
<html lang="fr">

<head>
    <!-- Head of the document -->
</head>
<body>
    ...
</body>

</html>
```

Voyons en détail ce que doit contenir cette balise `<head>`.

### Un titre

La première chose que doit contenir ta balise `<head>`, c'est **un titre** avec la balise `<title>`.

Le titre de la page **ne s'affichera pas directement** mais il sera visible sur les onglets et ce sera également le titre de notre page si un utilisateur met la page en favori.

![Capture d'écran d'un navigateur avec un onglet entouré avec le titre de la page](images/navigateur-titre-page.jpeg)
*Source:* [https://www.myprograming.com/html-head-tag/](https://www.myprograming.com/html-head-tag/)

Ce titre sera aussi celui utilisé par les moteurs de recherches lorsqu'ils indexeront ton site internet, d'où l'importance de toujours **être précis** lorsque tu ajoutes un titre.

La balise titre est un élément important du SEO (Search Engine Optimisation), c'est-à-dire de l'optimisation de ton site internet pour les moteurs de recherches.

Voici quelques conseils pour un titre SEO et user-friendly :

* Attention à la **longueur** du titre ! Un bon titre doit être **court, maximum 60 caractères**.

* Éviter de TOUT METTRE EN MAJUSCULE.

* Chaque page doit avoir un titre **unique** afin d'améliorer leur indexation.

* Utilise des caractères spéciaux comme `|` ou `-` pour séparer les éléments et faciliter la lecture : `Mot clef principal | Deuxième mot clef - Marque`

Voici quelques bons exemples de titre pour des pages HTML (note que ton `<head>` ne doit contenir qu'une seule balise `<title>`) :

```html
<title>Découvrez mon portfolio | Webdesigner Freelance - Bob Smith</title>
<title>Our products \| Delicious refreshing Juice - Minute Maid</title>
<title>Learn HTML5 \| Best courses - Wild Code School</title>
```

```xtext arrow
**🎯 À toi de jouer !**

Effectue quelques recherches sur google et regarde comment sont structurés les titres des pages web en fonction de tes recherches.

Note les titres qui attirent le plus ton oeil.

Ensuite, change le titre des pages que tu as créées dans le chapitre précédent en respectant les principes que tu as pu observer.

Note en commentaire la raison pour laquelle tu as choisi chacun des titres.
```

### Les métadonnées

La balise `<meta>` permet de transmettre des **informations pour le navigateur**.

Par exemple, utilisée avec l'attribut `charset` que nous avons vu dans la ressource précédente, il permet de **définir le jeu de caractères** (lettres et symboles) que tu veux utiliser pour ta page web.

Le jeu de caractères `utf-8` permet d'utiliser tous les caractères de n'importe quelle langue.

```html
<meta charset="UTF-8">
```

En réalité, si tu oublies de spécifier le jeu de caractères sur ton document HTML, la plupart des navigateurs utilisent automatiquement l'encodage des caractères utf-8 par défaut. Cependant, ajouter cette balise permet de s'assurer qu'avec tous les navigateurs et dans toutes les situations, ta page s'affichera avec le bon encodage de caractères.
{:.alert-info}

Tu peux également intégrer le **nom de l'auteur** d'une page web ainsi qu'une **description** à l'aide de la balise `<meta>` et de l'attribut `name`.

Ajouter le nom de l'auteur peut-être utile pour certains systèmes de gestion de contenus qui utilisent cette information.

```html
<meta name="author" content="Bob Smith">
```

La **description** est entre autres utilisée par les moteurs de recherches lorsqu'ils affichent un résultat avec ta page :

![Capture d'écran d'un résultat de recherche google avec la description entouré en rouge](images/google-description-resultat.webp)

```html
<meta name="description" content="Webdesigner, graphiste et developpeur frontend freelance, je désigne et développe des applications web innovantes et créatives !">
```

```xtext arrow
**🎯 À toi de jouer !**

Ajoute les métadonnées pour l'encodage des caractères (utf-8), l'auteur et la description de ta page.
```

### La favicône

Une favicône est une **icône utilisée par le navigateur pour représenter le site web**. Bien souvent, c'est une déclinaison du logo spécifiquement crée pour cette utilisation.

![Capture d'écran de la fenêtre du navigateur avec deux onglets et une favicône entouré sur chaque onglet](images/favicone-navigateur.jpeg)

Pour utiliser une favicône, tu dois créer une image au format **`.ico`** dont la taille est de **16x16.**

Pour convertir un PNG au format ico, tu peux utiliser un convertisseur en ligne comme [convertico](https://www.convertico.com/).

Ensuite, place la favicône à la racine de ton dossier de travail, puis ajoute la balise `<link>` avec 3 attributs :

* `rel` qui définit le type d'élément avec la valeur `shortcut icon`
* `href` qui spécifie l'emplacement de la favicône
* `type` qui spécifie le type du fichier avec la valeur `image/x-icon`

```html
<link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
```

Nous verrons plus tard que la balise `<link>` peut-être utilisée pour lier d'autres éléments comme des feuilles de style par exemple.

```xtext arrow
**🎯 À toi de jouer !**

Ajoute une favicône dans ton dossier et ajoute la balise sur toutes les pages de ton projet.
```

## Récapitulatif

* La balise `<head>` contient de nombreuses métadonnées utiles pour le navigateur.

* Ajouter un titre à sa page HTML est très important, tant pour l'expérience utilisateur que pour améliorer le SEO. Le titre doit être clair, impactant et différent pour chaque page du site web.

* La balise `<meta>` permet d'ajouter des métadonnées, utiles également pour les moteurs de recherches.

* La favicône est une petite icône qui s'affiche sur le navigateur, il est important de l'ajouter à l'aide de la balise `<link>`

## Challenge

Mets en forme le travail que tu as réalisé durant cette ressource et compare le résultat avec la solution qui est proposée !

### Critères de validation

* [ ] Les pages contiennent un titre clair, respectant les principes évoqués dans la ressource ainsi qu'un commentaire expliquant le choix réalisé.
* [ ] Toutes les balises `<meta>` sont présentes
* [ ] La favicône s'affiche bien

[Voir la solution](solution.md){:.alert-info}
