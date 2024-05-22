# Exercice de routing

L'objectif de cet exercice est de créer une application Angular avec du routage pour naviguer entre différentes vues. Vous allez apprendre à configurer les routes, utiliser les composants et gérer des routes dynamiques. 

#### Étape 1 : Créer les composants

1. **Créer trois composants** :
   - Ouvrez votre terminal et exécutez :
     ```bash
     ng generate component home
     ng generate component about
     ng generate component task-detail
     ```

2. **Définir le contenu des composants** :
   - Dans `home.component.html` et `about.component.html`, ajoutez du contenu.

#### Fichier : `home.component.html`

```html
<h2>Home</h2>
<p>Welcome to the home page!</p>
```

#### Fichier : `about.component.html`

```html
<h2>About</h2>
<p>This is the about page.</p>
```

#### Étape 2 : Configurer le routage

1. **Modifiez le fichier pour configurer les routes** :
   - Modifiez le fichier `app.routes.ts` à la racine de votre projet et configurez les routes comme suit :

#### Fichier : `app.routes.ts`

```typescript
path 'home' --> HomeComponent
path 'about' --> AboutComponent
path 'task/:id' --> TaskDetailsComponent

*Bonus:
path '' --> redirect to 'home'
path 404 --> NotFoundComponent
```

2. **Configurer les routes dans le composant principal** :
   - Modifiez `app.component.ts` pour utiliser les routes et ajouter des liens de navigation dans le template.

#### Étape 3 : Gérer les routes dynamiques

1. **Modifier le fichier `task-detail.component.ts` pour gérer les routes dynamiques** :

#### Fichier : `task-detail.component.ts`

```typescript
Chercher ActivatedRoute
```

2. **Définir le contenu du template pour afficher le contenu en fonction de l'ID** :

#### Fichier : `task-detail.component.html`

```html
<p>Task Detail: {{ taskId }}</p>
```

#### Étape 4 : Exécuter et tester l'application

1. **Tester l'application** :
   - Lancez votre application avec `ng serve`.
   - Vérifiez que vous pouvez naviguer entre la page d'accueil (Home), la page À propos (About), et les détails des tâches (Task 1, Task 2) via des routes dynamiques.

### Résultat attendu

Vous devriez avoir une application Angular avec une barre de navigation permettant de passer de la page d'accueil à la page À propos, et aux détails de différentes tâches via des routes dynamiques.

### Points à retenir

- Comment définir et naviguer entre différentes routes, y compris des routes dynamiques.
