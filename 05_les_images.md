# Les Images en HTML

Les images sont des éléments importants des pages web, ajoutant du contenu visuel et améliorant l'expérience utilisateur. En HTML, les images sont insérées à l'aide de la balise `<img>`. Voici un aperçu détaillé de l'utilisation des images en HTML.

## Table des matières

- [Définition et syntaxe de base](#définition-et-syntaxe-de-base)
- [Attributs de la balise `<img>`](#attributs-de-la-balise-img)
- [Images réactives](#images-réactives)
- [Images et accessibilité](#images-et-accessibilité)
- [Images en arrière-plan](#images-en-arrière-plan)
- [Bonnes pratiques](#bonnes-pratiques)
- [Exemple complet](#exemple-complet)

## Définition et syntaxe de base

La balise `<img>` est utilisée pour insérer des images dans un document HTML. Elle est autonome, c'est-à-dire qu'elle n'a pas de balise de fermeture.

```html
<img src="chemin/vers/image.jpg" alt="Description de l'image" />
```

## Attributs de la balise `<img>`

- **`src`** : Spécifie le chemin vers l'image. Il peut s'agir d'un chemin relatif ou absolu.

```html
<img src="images/photo.jpg" alt="Photo de paysage" />
```

- **`alt`** : Fournit un texte alternatif pour l'image. C'est essentiel pour l'accessibilité et le SEO.

```html
<img src="images/photo.jpg" alt="Photo de paysage au coucher du soleil" />
```

- **`width` et `height`** : Spécifient la largeur et la hauteur de l'image en pixels.

```html
<img src="images/photo.jpg" alt="Photo de paysage" width="600" height="400" />
```

- **`title`** : Fournit des informations supplémentaires sur l'image. Ce texte apparaît généralement comme une info-bulle lorsque l'utilisateur passe la souris sur l'image.

```html
<img
  src="images/photo.jpg"
  alt="Photo de paysage"
  title="Coucher du soleil sur un paysage"
/>
```

## Images réactives

Pour rendre les images réactives, vous pouvez utiliser des techniques CSS afin que les images s'ajustent à la taille de l'écran.

```html
<style>
  img {
    max-width: 100%;
    height: auto;
  }
</style>

<img src="images/photo.jpg" alt="Photo de paysage" />
```

## Images et accessibilité

Utiliser l'attribut `alt` est crucial pour rendre les images accessibles aux utilisateurs de lecteurs d'écran. Si l'image est purement décorative, vous pouvez laisser l'attribut `alt` vide (`alt=""`).

```html
<img src="images/decorative.jpg" alt="" />
```

## Images en arrière-plan

Les images en arrière-plan sont souvent utilisées dans les feuilles de style CSS plutôt que directement dans le HTML.

```html
<!DOCTYPE html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Exemple d'Image de Fond</title>
    <style>
      .background {
        background-image: url("images/background.jpg");
        background-size: cover;
        height: 500px;
      }
    </style>
  </head>
  <body>
    <div class="background">
      <h1>Texte sur une image de fond</h1>
    </div>
  </body>
</html>
```

## Bonnes pratiques

- **Utilisez des images optimisées** : Réduisez la taille des fichiers images pour améliorer les temps de chargement des pages.
- **Fournissez un texte alternatif significatif** : Décrivez le contenu et la fonction de l'image.
- **Utilisez des formats appropriés** : Les formats JPEG, PNG, GIF et WebP sont les plus courants. Utilisez JPEG pour les photos, PNG pour les images avec des transparences, et WebP pour une meilleure compression.
- **Évitez les images purement décoratives avec des `alt` non significatifs** : Utilisez `alt=""` pour les images décoratives afin de ne pas distraire les utilisateurs de lecteurs d'écran.

## Exemple complet

Voici un exemple complet montrant l'utilisation des différentes fonctionnalités des images en HTML.

```html
<!DOCTYPE html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Exemples d'Images en HTML</title>
    <style>
      .responsive-img {
        max-width: 100%;
        height: auto;
      }
      .background {
        background-image: url("images/background.jpg");
        background-size: cover;
        height: 500px;
      }
    </style>
  </head>
  <body>
    <h1>Exemples d'Images</h1>

    <h2>Image de Base</h2>
    <img src="images/photo.jpg" alt="Photo de paysage au coucher du soleil" />

    <h2>Image avec Dimensions Spécifiées</h2>
    <img
      src="images/photo.jpg"
      alt="Photo de paysage"
      width="600"
      height="400"
    />

    <h2>Image Réactive</h2>
    <img src="images/photo.jpg" alt="Photo de paysage" class="responsive-img" />

    <h2>Image avec Titre</h2>
    <img
      src="images/photo.jpg"
      alt="Photo de paysage"
      title="Coucher du soleil sur un paysage"
    />

    <h2>Image Purement Décorative</h2>
    <img src="images/decorative.jpg" alt="" />

    <h2>Image en Arrière-Plan</h2>
    <div class="background">
      <h1>Texte sur une image de fond</h1>
    </div>
  </body>
</html>
```

En suivant ces pratiques et en utilisant les différentes fonctionnalités des balises `<img>`, vous pouvez créer des pages web visuellement attractives et accessibles. Continuez à expérimenter pour renforcer vos compétences en HTML.
