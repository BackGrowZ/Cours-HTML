# Introduction au HTML

HTML (HyperText Markup Language) est le langage standard utilisé pour créer des pages web. Il est utilisé pour structurer le contenu de la page en définissant des éléments tels que les titres, les paragraphes, les liens, les images, et bien plus encore. Ce cours vous donnera une base solide pour comprendre et utiliser HTML pour créer des pages web.

## Table des matières

1. [Structure de base d'un document HTML](#structure-de-base-dun-document-html)
2. [Éléments de texte](#éléments-de-texte)
3. [Liens et images](#liens-et-images)
4. [Listes](#listes)
5. [Tables](#tables)
6. [Formulaires](#formulaires)
7. [Éléments de multimédia](#éléments-de-multimédia)
8. [Exemples et Pratique](#exemples-et-pratique)

## Structure de base d'un document HTML

Chaque document HTML commence par une déclaration de type de document `<!DOCTYPE html>`, suivie par l'élément `<html>`, qui contient les éléments `<head>` et `<body>`.

```html
<!DOCTYPE html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Titre de la Page</title>
  </head>
  <body>
    <h1>Bienvenue sur ma page web</h1>
    <p>Ceci est un paragraphe.</p>
  </body>
</html>
```

## Éléments de texte

Les éléments de texte sont utilisés pour définir les titres, les paragraphes, et autres textes.

```html
<h1>Titre de niveau 1</h1>
<h2>Titre de niveau 2</h2>
<p>Ceci est un paragraphe.</p>
<strong>Texte en gras</strong>
<em>Texte en italique</em>
```

## Liens et images

Les liens permettent de naviguer entre les pages web, et les images ajoutent du contenu visuel.

```html
<a href="https://www.example.com">Ceci est un lien</a>
<img src="image.jpg" alt="Description de l'image" />
```

## Listes

HTML supporte deux types de listes : les listes ordonnées et les listes non ordonnées.

```html
<!-- Liste non ordonnée -->
<ul>
  <li>Élément de liste 1</li>
  <li>Élément de liste 2</li>
  <li>Élément de liste 3</li>
</ul>

<!-- Liste ordonnée -->
<ol>
  <li>Premier élément</li>
  <li>Deuxième élément</li>
  <li>Troisième élément</li>
</ol>
```

## Tables

Les tables permettent de structurer les données en lignes et colonnes.

```html
<table>
  <thead>
    <tr>
      <th>En-tête 1</th>
      <th>En-tête 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Donnée 1</td>
      <td>Donnée 2</td>
    </tr>
    <tr>
      <td>Donnée 3</td>
      <td>Donnée 4</td>
    </tr>
  </tbody>
</table>
```

## Formulaires

Les formulaires permettent de recueillir des données utilisateur via des champs de saisie, des cases à cocher, des boutons radio, et d'autres éléments de formulaire.

```html
<form action="/soumettre" method="post">
  <label for="nom">Nom :</label>
  <input type="text" id="nom" name="nom" />

  <label for="email">Email :</label>
  <input type="email" id="email" name="email" />

  <input type="submit" value="Envoyer" />
</form>
```

## Éléments de multimédia

HTML5 permet d'intégrer facilement des vidéos et des fichiers audio.

```html
<!-- Vidéo -->
<video controls>
  <source src="video.mp4" type="video/mp4" />
  Votre navigateur ne supporte pas la vidéo HTML5.
</video>

<!-- Audio -->
<audio controls>
  <source src="audio.mp3" type="audio/mp3" />
  Votre navigateur ne supporte pas l'audio HTML5.
</audio>
```

## Exemples et Pratique

Pour bien maîtriser HTML, il est recommandé de pratiquer en créant diverses pages web, en utilisant les différents éléments vus précédemment, et en expérimentant avec des structures de plus en plus complexes.

### Exemple Complet

```html
<!DOCTYPE html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Exemple Complet de Page HTML</title>
  </head>
  <body>
    <header>
      <h1>Ma Page Web</h1>
      <nav>
        <ul>
          <li><a href="#section1">Section 1</a></li>
          <li><a href="#section2">Section 2</a></li>
          <li><a href="#section3">Section 3</a></li>
        </ul>
      </nav>
    </header>
    <main>
      <section id="section1">
        <h2>Section 1</h2>
        <p>Bienvenue dans la section 1 de ma page web.</p>
      </section>
      <section id="section2">
        <h2>Section 2</h2>
        <p>Bienvenue dans la section 2 de ma page web.</p>
        <img src="image.jpg" alt="Description de l'image" />
      </section>
      <section id="section3">
        <h2>Section 3</h2>
        <p>Bienvenue dans la section 3 de ma page web.</p>
        <ul>
          <li>Élément de liste 1</li>
          <li>Élément de liste 2</li>
          <li>Élément de liste 3</li>
        </ul>
      </section>
    </main>
    <footer>
      <p>&copy; 2024 Mon Site Web</p>
    </footer>
  </body>
</html>
```
