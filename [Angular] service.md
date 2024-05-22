# exercice_service_angular
### Consignes de l'exercice

L'objectif de cet exercice est de créer une application Angular pour gérer une liste de tâches (todo list) en utilisant un service. Conseil: faire quelques recherches sur l'utilisation de `[(ngModel)]` pour lier des données dans un formulaire.

#### Étape 1 : Créer le service Todo

1. **Créer un service** :
   - Ouvrez votre terminal et exécutez :
     ```bash
     ng generate service services/todo
     ```
   - Dans `todo.service.ts`, définissez une liste de tâches privée et ajoutez deux méthodes : `getTodos` (pour récupérer les tâches) et `addTodo` (pour en ajouter une nouvelle).

#### Étape 2 : Créer le composant TodoList

1. **Créer un composant standalone** :
   - Exécutez :
     ```bash
     ng generate component todo-list
     ```
   - Dans `todo-list.component.ts`, importez `TodoService` et utilisez-le pour gérer les tâches.

#### Étape 3 : Utiliser les nouvelles fonctionnalités Angular

1. **Afficher les tâches** :
   - Utilisez la syntaxe `@for` dans le template HTML pour afficher les tâches.
   - Exemple de syntaxe `@for` : `@for (let item of items; track item.id) { <div>{{ item }}</div> }`

2. **Ajouter une nouvelle tâche** :
   - Ajoutez un champ de saisie et un bouton dans le template pour permettre l'ajout de nouvelles tâches.
   - Utilisez `[(ngModel)]` pour lier la saisie de l'utilisateur à une propriété de votre composant.
   - Faites des recherches sur `[(ngModel)]` si nécessaire.

#### Étape 4 : Intégrer le composant dans l'application

1. **Intégrer le composant** :
   - Dans `app.component.ts`, importez et affichez `TodoListComponent` dans le template.

#### Étape 5 : Exécuter et tester l'application

1. **Tester l'application** :
   - Lancez votre application avec `ng serve` et vérifiez que vous pouvez voir et ajouter des tâches à la liste.
