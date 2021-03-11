# Résultats du W3C validator
## Commentaires généraux
 * Les enfants d'une liste `<ul>` ou `<ol>` __doivent__ être des éléments de liste `<li>`. Il n'y a pas de raison de placer une `<div>` ici ; il s'agit du titre qui précède la liste et devrait donc se trouver avant. (Menu de navigation, sommaire)
 * Les espaces dans les noms de page et de fichier sont à éviter.

## Page personnages 
* L'utilisation de l'attribut `border` des tableaux HTML est à déconseiller ; il vaut mieux utiliser CSS pour régler la bordure. (Non pénalisé car vu au cours)

# Utilisation d'HTML
 * Dans la page Gameplay, il vaudrait mieux séparer le texte en plusieurs paragraphes `<p>`, plutôt que d'avoir un seul paragraphe unique et des retours à la ligne. De même il vaudrait mieux placer la `<div id="gameplay">` entre deux paragraphes.
 * Dans cette même page, pourquoi utiliser des titres `<h1>`, `<h2>` et `<h3>` ? Ces balises servent de titres pour créer des sous-sections, mais les trois sections semblent ici se place au même niveau (ou du moins les sections "Intérêt" et "Auteur et développeur de la série").
 * Essaie d'utiliser des noms d'identifiants cohérents, par exemple dans les miniatures sur la page Personnages (`marioPiti`, `yoshi`, `RDD` ; il n'est pas immédiatement apparent qu'il s'agit d'objets similaires)
 * Pas de `<header>` dans la page de commentaires

# Utilisation de CSS
 * Tu as du code CSS redondant : plusieurs pages utilisent le même style global, et il aurait mieux valu utiliser un fichier séparé commun chargé par toutes les pages. Cela t'aurait aussi permis d'avoir la même allure de site sur toutes les pages ("Commentaire" a une allure très différente des autres)
 * Le rendu du tableau dans la page "personnages principaux" est difficile sur certains écrans. Par exemple sur un écran de résolution 1400x900, le tableau dépasse en largeur et le contenu de la page dans son ensemble suit. Il pourrait être intéressant de régler la largeur des images pour s'adapter à la largeur de l'écran, par exemple avec `max-width`.

# Grille d'évaluation
| Critère           | Sur | Cote |
| :---------------- | :-: |:---: |
| 3 pages           |  1  |  1   |
| En-tête           |  1  | 0.5  |
| Pied de page      |  1  |  1   |
| Footer (contenu)  |  1  |  1   |
| Menu nav          |  3  |  2   |
| Balises HTML      |  3  | 1.5  |
| grid              |  3  |  3   |
| flex              |  2  |  2   |
| Police            |  1  |  1   |
| Propriétés CSS    |  3  |  2   |
| Rendu correct     |  1  | 0.5  |
| __Total__        |__20__|__16__|
