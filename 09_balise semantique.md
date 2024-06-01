### Les Balises Sémantiques en HTML

Les balises sémantiques en HTML décrivent le sens (ou la sémantique) du contenu qu'elles renferment, ce qui rend le code plus lisible et compréhensible, tant pour les développeurs que pour les moteurs de recherche. Ces balises contribuent également à l'accessibilité des pages web. Voici un aperçu des balises sémantiques les plus courantes en HTML5.

## Table des matières

- [Définition et importance des balises sémantiques](#définition-et-importance-des-balises-sémantiques)
- [Les balises sémantiques courantes](#les-balises-sémantiques-courantes)
  - [La balise `<header>`](#la-balise-header)
  - [La balise `<nav>`](#la-balise-nav)
  - [La balise `<main>`](#la-balise-main)
  - [La balise `<section>`](#la-balise-section)
  - [La balise `<article>`](#la-balise-article)
  - [La balise `<aside>`](#la-balise-aside)
  - [La balise `<footer>`](#la-balise-footer)
  - [La balise `<figure>` et `<figcaption>`](#la-balise-figure-et-figcaption)
  - [La balise `<mark>`](#la-balise-mark)
- [Bonnes pratiques](#bonnes-pratiques)
- [Exemple complet](#exemple-complet)

## Définition et importance des balises sémantiques

Les balises sémantiques apportent du sens au contenu qu'elles enveloppent. Contrairement aux balises non-sémantiques comme `<div>` et `<span>`, qui n'apportent aucune information sur le type de contenu qu'elles contiennent, les balises sémantiques permettent de structurer le document de manière logique.

## Les balises sémantiques courantes

### La balise `<header>`

La balise `<header>` est utilisée pour regrouper le contenu d'en-tête d'une page ou d'une section. Elle peut contenir des éléments comme des titres, des logos, des menus de navigation, etc.

```html
<header>
  <h1>Bienvenue sur mon site</h1>
  <nav>
    <ul>
      <li><a href="#home">Accueil</a></li>
      <li><a href="#about">À propos</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>
```

### La balise `<nav>`

La balise `<nav>` est utilisée pour regrouper les liens de navigation.

```html
<nav>
  <ul>
    <li><a href="#home">Accueil</a></li>
    <li><a href="#about">À propos</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>
```

### La balise `<main>`

La balise `<main>` est utilisée pour envelopper le contenu principal d'une page, unique et directement lié au sujet principal de la page.

```html
<main>
  <h2>Articles Récents</h2>
  <article>
    <h3>Titre de l'article</h3>
    <p>Contenu de l'article...</p>
  </article>
</main>
```

### La balise `<section>`

La balise `<section>` est utilisée pour regrouper les contenus thématiquement liés. Chaque section devrait idéalement avoir un titre.

```html
<section id="about">
  <h2>À propos de nous</h2>
  <p>Informations sur notre entreprise...</p>
</section>
```

### La balise `<article>`

La balise `<article>` est utilisée pour des contenus indépendants pouvant être distribués ou réutilisés indépendamment, comme des articles de blog, des articles de presse, des commentaires, etc.

```html
<article>
  <h2>Titre de l'article</h2>
  <p>Contenu de l'article...</p>
</article>
```

### La balise `<aside>`

La balise `<aside>` est utilisée pour le contenu secondaire ou complémentaire, souvent utilisé pour les barres latérales, les blocs d'information connexes, etc.

```html
<aside>
  <h2>Informations Complémentaires</h2>
  <p>Des informations supplémentaires ou connexes...</p>
</aside>
```

### La balise `<footer>`

La balise `<footer>` est utilisée pour le pied de page d'une page ou d'une section. Elle peut contenir des informations de copyright, des liens vers des politiques de confidentialité, des liens de contact, etc.

```html
<footer>
  <p>&copy; 2024 Mon Site Web. Tous droits réservés.</p>
  <nav>
    <ul>
      <li><a href="#privacy">Politique de confidentialité</a></li>
      <li><a href="#terms">Conditions d'utilisation</a></li>
    </ul>
  </nav>
</footer>
```

### La balise `<figure>` et `<figcaption>`

La balise `<figure>` est utilisée pour les contenus illustratifs comme des images, des graphiques, etc., et la balise `<figcaption>` pour ajouter une légende à ces contenus.

```html
<figure>
  <img src="image.jpg" alt="Description de l'image" />
  <figcaption>Légende de l'image</figcaption>
</figure>
```

### La balise `<mark>`

La balise `<mark>` est utilisée pour mettre en évidence le texte pertinent.

```html
<p>Ceci est un <mark>texte mis en évidence</mark> dans un paragraphe.</p>
```

## Bonnes pratiques

- **Utilisez des balises sémantiques appropriées** : Choisissez la balise qui décrit le mieux le contenu qu'elle enveloppe.
- **Évitez l'abus des balises sémantiques** : N'utilisez pas une balise sémantique uniquement pour ses propriétés de style. Utilisez les balises en fonction de leur sens.
- **Améliorez l'accessibilité** : Les balises sémantiques aident les technologies d'assistance à comprendre la structure de votre page, rendant votre site plus accessible.
- **Optimisez le SEO** : Les moteurs de recherche utilisent la structure sémantique pour indexer et classer le contenu, améliorant ainsi le référencement de votre site.

## Exemple complet

Voici un exemple complet utilisant diverses balises sémantiques pour structurer une page HTML.

```html
<!DOCTYPE html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Exemple de Balises Sémantiques</title>
  </head>
  <body>
    <header>
      <h1>Bienvenue sur mon site</h1>
      <nav>
        <ul>
          <li><a href="#home">Accueil</a></li>
          <li><a href="#about">À propos</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </header>
    <main>
      <section id="about">
        <h2>À propos de nous</h2>
        <p>Informations sur notre entreprise...</p>
      </section>
      <section>
        <h2>Articles Récents</h2>
        <article>
          <h3>Titre de l'article</h3>
          <p>Contenu de l'article...</p>
        </article>
      </section>
    </main>
    <aside>
      <h2>Informations Complémentaires</h2>
      <p>Des informations supplémentaires ou connexes...</p>
    </aside>
    <footer>
      <p>&copy; 2024 Mon Site Web. Tous droits réservés.</p>
      <nav>
        <ul>
          <li><a href="#privacy">Politique de confidentialité</a></li>
          <li><a href="#terms">Conditions d'utilisation</a></li>
        </ul>
      </nav>
    </footer>
  </body>
</html>
```

En utilisant ces balises sémantiques, vous pouvez créer des pages web plus structurées, accessibles et optimisées pour le référencement. Continuez à expérimenter pour renforcer vos compétences en HTML.
