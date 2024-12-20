* Créez une application de gestion de recettes de cuisine permettant aux utilisateurs de visualiser et gérer leurs recettes préférées.

* Structure des données requise :
  - Créez une interface `Recipe` avec les propriétés : id, name, description, ingredients
  - Créez une interface `Ingredient` avec les propriétés : id, name, quantity, unit

* Exigences techniques :
  - Développez un service `RecipeService` qui gérera la logique de gestion des recettes
  - Implémentez l'injection de dépendance du service dans les composants nécessaires avec inject
  - Utilisez la directive `@for` pour afficher la liste des recettes et leurs ingrédients

* Structure minimale de l'application :
  - Un composant principal `RecipeList` affichant toutes les recettes
  - Un service `RecipeService` avec une propriété `recipes` qui contient les recettes
