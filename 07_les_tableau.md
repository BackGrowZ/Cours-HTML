# Les Tableaux en HTML

Les éléments `<thead>`, `<tbody>`, et `<tfoot>` sont utilisés pour structurer les tableaux en HTML. Ils permettent de séparer logiquement les en-têtes de tableau des données de tableau, ce qui améliore la lisibilité et l'accessibilité.

## Table des matières

- [Définition et syntaxe de base](#définition-et-syntaxe-de-base)
- [Utilisation de `<thead>`](#utilisation-de-thead)
- [Utilisation de `<tbody>`](#utilisation-de-tbody)
- [Utilisation de `<tfoot>`](#utilisation-de-tfoot)
- [Exemple complet](#exemple-complet)

## Définition et syntaxe de base

Un tableau en HTML est défini avec la balise `<table>`. Les lignes de tableau sont définies avec la balise `<tr>`, les cellules d'en-tête avec la balise `<th>`, et les cellules de données avec la balise `<td>`.

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

## Utilisation de `<thead>`

L'élément `<thead>` est utilisé pour regrouper les lignes d'en-tête d'un tableau. Cela permet aux navigateurs et aux technologies d'assistance de traiter correctement les en-têtes de tableau.

```html
<table>
  <thead>
    <tr>
      <th>Nom</th>
      <th>Âge</th>
      <th>Profession</th>
    </tr>
  </thead>
</table>
```

## Utilisation de `<tbody>`

L'élément `<tbody>` est utilisé pour regrouper les lignes de données du tableau. Un tableau peut contenir plusieurs éléments `<tbody>` si nécessaire.

```html
<table>
  <thead>
    <tr>
      <th>Nom</th>
      <th>Âge</th>
      <th>Profession</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Alice</td>
      <td>30</td>
      <td>Ingénieure</td>
    </tr>
    <tr>
      <td>Bob</td>
      <td>25</td>
      <td>Designer</td>
    </tr>
  </tbody>
</table>
```

## Utilisation de `<tfoot>`

L'élément `<tfoot>` est utilisé pour regrouper les lignes de pied de tableau. Cela permet de placer des totaux ou d'autres informations de résumé à la fin du tableau.

```html
<table>
  <thead>
    <tr>
      <th>Nom</th>
      <th>Âge</th>
      <th>Profession</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Alice</td>
      <td>30</td>
      <td>Ingénieure</td>
    </tr>
    <tr>
      <td>Bob</td>
      <td>25</td>
      <td>Designer</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="3">Total : 2 employés</td>
    </tr>
  </tfoot>
</table>
```

## Exemple complet

Voici un exemple complet montrant l'utilisation de `<thead>`, `<tbody>`, et `<tfoot>` dans un tableau HTML.

```html
<!DOCTYPE html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Exemples de Tableaux en HTML</title>
  </head>
  <body>
    <h1>Exemples de Tableaux</h1>

    <h2>
      Tableau Structuré avec `
      <thead>
        `, `
      </thead>
      <tbody>
        `, et `
      </tbody>
      <tfoot>
        `
      </tfoot>
    </h2>
    <table border="1">
      <thead>
        <tr>
          <th>Nom</th>
          <th>Âge</th>
          <th>Profession</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Alice</td>
          <td>30</td>
          <td>Ingénieure</td>
        </tr>
        <tr>
          <td>Bob</td>
          <td>25</td>
          <td>Designer</td>
        </tr>
      </tbody>
      <tfoot>
        <tr>
          <td colspan="3">Total : 2 employés</td>
        </tr>
      </tfoot>
    </table>

    <h2>Tableau avec Fusion de Cellules</h2>
    <table border="1">
      <thead>
        <tr>
          <th colspan="2">Titre fusionné</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Donnée 1</td>
          <td>Donnée 2</td>
        </tr>
        <tr>
          <th rowspan="2">Titre fusionné</th>
          <td>Donnée 1</td>
        </tr>
        <tr>
          <td>Donnée 2</td>
        </tr>
      </tbody>
    </table>

    <h2>Tableau avec Légende</h2>
    <table border="1">
      <caption>
        Liste des employés
      </caption>
      <thead>
        <tr>
          <th>Nom</th>
          <th>Âge</th>
          <th>Profession</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Alice</td>
          <td>30</td>
          <td>Ingénieure</td>
        </tr>
        <tr>
          <td>Bob</td>
          <td>25</td>
          <td>Designer</td>
        </tr>
      </tbody>
    </table>

    <h2>Tableaux Imbriqués</h2>
    <table border="1">
      <thead>
        <tr>
          <th>Nom</th>
          <th>Détails</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Alice</td>
          <td>
            <table border="1">
              <thead>
                <tr>
                  <th>Âge</th>
                  <td>30</td>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <th>Profession</th>
                  <td>Ingénieure</td>
                </tr>
              </tbody>
            </table>
          </td>
        </tr>
        <tr>
          <td>Bob</td>
          <td>
            <table border="1">
              <thead>
                <tr>
                  <th>Âge</th>
                  <td>25</td>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <th>Profession</th>
                  <td>Designer</td>
                </tr>
              </tbody>
            </table>
          </td>
        </tr>
      </tbody>
    </table>
  </body>
</html>
```

En utilisant `<thead>`, `<tbody>`, et `<tfoot>`, vous pouvez créer des tableaux HTML bien structurés et accessibles. Continuez à expérimenter pour renforcer vos compétences en HTML.
