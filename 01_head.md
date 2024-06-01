# La Balise `<head>` et ses Contenus

La balise `<head>` est une partie essentielle d'un document HTML. Elle contient des méta-informations sur le document, qui ne sont pas directement affichées à l'utilisateur, mais qui sont cruciales pour le bon fonctionnement de la page et pour les moteurs de recherche. Explorons les différentes balises que vous pouvez trouver à l'intérieur de la balise `<head>`.

## Table des matières

- [La balise `<title>`](#la-balise-title)
- [Les balises `<meta>`](#les-balises-meta)
- [La balise `<link>`](#la-balise-link)
- [La balise `<style>`](#la-balise-style)
- [La balise `<script>`](#la-balise-script)
- [Exemple Complet](#exemple-complet)

## La balise `<title>`

La balise `<title>` définit le titre du document, qui apparaît dans l'onglet du navigateur et dans les résultats des moteurs de recherche.

```html
<head>
  <title>Ma Page Web</title>
</head>
```

## Les balises `<meta>`

Les balises `<meta>` fournissent des métadonnées sur le document HTML, telles que l'encodage des caractères, la description de la page, et les mots-clés.

- **Encodage des caractères** : Définit l'encodage des caractères utilisé par le document. UTF-8 est l'encodage le plus couramment utilisé.

```html
<meta charset="UTF-8" />
```

- **Description** : Fournit une description de la page pour les moteurs de recherche.

```html
<meta name="description" content="Ceci est une description de ma page web." />
```

- **Mots-clés** : Fournit une liste de mots-clés pertinents pour le contenu de la page.

```html
<meta name="keywords" content="HTML, CSS, JavaScript, Tutoriel" />
```

- **Viewport** : Contrôle la mise en page sur les navigateurs mobiles, notamment pour le responsive design.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

- **Auteur** : Indique l'auteur du document.

```html
<meta name="author" content="Votre Nom" />
```

## La balise `<link>`

La balise `<link>` est utilisée pour lier des ressources externes, comme des feuilles de style CSS, des icônes, ou des polices de caractères.

- **Feuilles de style CSS** : Lien vers une feuille de style externe.

```html
<link rel="stylesheet" href="styles.css" />
```

- **Favicon** : Lien vers une icône de site (favicon).

```html
<link rel="icon" href="favicon.ico" type="image/x-icon" />
```

## La balise `<style>`

La balise `<style>` permet d'inclure des styles CSS directement dans le document HTML.

```html
<style>
  body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
  }
</style>
```

## La balise `<script>`

La balise `<script>` permet d'inclure ou de référencer des scripts JavaScript.

- **Script interne** : JavaScript inclus directement dans le document HTML.

```html
<script>
  console.log("Hello, world!");
</script>
```

- **Script externe** : Lien vers un fichier JavaScript externe.

```html
<script src="script.js"></script>
```

## Exemple Complet

Voici un exemple complet de la balise `<head>` incluant toutes les balises mentionnées :

```html
<!DOCTYPE html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta
      name="description"
      content="Ceci est une description de ma page web."
    />
    <meta name="keywords" content="HTML, CSS, JavaScript, Tutoriel" />
    <meta name="author" content="Votre Nom" />
    <title>Ma Page Web</title>
    <link rel="stylesheet" href="styles.css" />
    <link rel="icon" href="favicon.ico" type="image/x-icon" />
    <style>
      body {
        font-family: Arial, sans-serif;
        background-color: #f0f0f0;
      }
    </style>
    <script>
      console.log("Hello, world!");
    </script>
    <script src="script.js"></script>
  </head>
  <body>
    <h1>Bienvenue sur ma page web</h1>
    <p>Ceci est un paragraphe.</p>
  </body>
</html>
```

En comprenant et en utilisant correctement les balises dans le `<head>`, vous pouvez améliorer la performance, l'accessibilité, et le référencement de vos pages web. Continuez à expérimenter avec ces balises pour voir comment elles affectent vos documents HTML.
