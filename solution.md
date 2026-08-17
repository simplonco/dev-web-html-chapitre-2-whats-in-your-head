---
title: HTML - Chapitre 2 | What's in your &lt;head&gt; ? - Solution
description: HTML - Chapitre 2 | What's in your &lt;head&gt; ? - Solution
show_toc: true
parent: HTML - Chapitre 2 | What's in your &lt;head&gt; ?
---

## Pour le fichier index.html

```html
<!DOCTYPE html>
<html lang="fr">

<head>
    <title>Bienvenue sur mon site internet | Bob Smith Webdesigner</title>
    <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
    <meta name="author" content="Bob Smith">
    <meta name="description"
        content="Webdesigner, graphiste et developpeur frontend freelance, je désigne et développe des applications web innovantes et créatives !">
</head>

<body>
    <h1>Hello world!</h1>
    <h2>Welcome here</h2>
    <p>Bienvenue sur mon <strong>incroyable</strong> site internet!</p>
    <p>Je m'appelle Bob</p>
    <img src="https://placekitten.com/200/287" alt="" width="300" />
    <button disabled="true">Click here</button>
    <a href="about.html">À propos de moi</a>
</body>

</html>
```

## Pour le fichier about.html

```html
<!DOCTYPE html>
<html lang="fr">

<head>
        <title>Découvrez-en plus sur moi | Bob Smith Webdesigner</title>
        <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
        <meta name="author" content="Bob Smith">
        <meta name="description"
            content="Webdesigner, graphiste et developpeur frontend freelance, je désigne et développe des  applications web innovantes et créatives !">
</head>

<body>
    <h1>A propos de moi:</h1>

    <h2>Mes skills :</h2>
    <ul>
        <li>HTML</li>
        <li>Webdesign</li>
        <li>Illustration</li>
        <li>Piano</li>
    </ul>

    <h2>Mes plats préférés</h2>
    <ol>
        <li>Pizza</li>
        <li>Sushi</li>
        <li>Burgers</li>
    </ol>

    <a href="index.html">Retourner à l'accueil</a>
</body>

</html>
```
