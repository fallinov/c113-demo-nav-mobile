# C113 — Démo responsive : la navigation mobile d'abord

Exercice du cours 113 (séance 11) : la barre de navigation de la séance 9 passe en mobile-first.

Ce dépôt contient le **code de départ** : la barre de navigation terminée, pensée pour le grand
écran. Sur téléphone, les liens passent simplement à la ligne.

## Démarrer

1. En haut de cette page : **Use this template → Create a new repository**. Choisis ton compte
   comme propriétaire et laisse *Include all branches* décoché : tu obtiens **ta propre copie**,
   sur laquelle tu peux faire commit et push.
2. Dans WebStorm : **File → New → Project from Version Control**, colle l'URL de **ta copie**.
3. Ouvre `index.html` dans Brave ou Firefox, avec la vue mobile des DevTools à 375 px de large.
4. Écris ton CSS dans `style.css`, une étape après l'autre, et recharge la page à chaque fois.

## Les étapes

| Étape | À faire | Propriétés |
|-------|---------|------------|
| 1 | Menu : un lien par ligne | `flex-direction: column` sur `.menu`, retirer `flex-wrap` |
| 2 | Header : le logo, puis le menu en dessous | `flex-direction: column` sur `.header`, retirer `justify-content`, `align-items` et `flex-wrap` |
| 3 | Dès 768 px de large, repasser en ligne | `@media (min-width: 768px)`, `flex-direction: row`, `justify-content`, `align-items` |

Teste à 375 px, puis élargis la fenêtre au-delà de 768 px.

## La solution

Elle est sur la branche
[`solution`](https://github.com/fallinov/c113-demo-nav-mobile/tree/solution) de ce dépôt :
[voir les commits](https://github.com/fallinov/c113-demo-nav-mobile/commits/solution/).

## S'entraîner

- Nuxy, module 12 : [Le menu qui s'empile](https://www.nuxy.ch/exercises/css-menu-responsive)
- Plan de la séance : https://devjs.ch/cours/113/plan#seance-11-11-novembre-2026
