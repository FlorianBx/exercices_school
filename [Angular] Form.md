# Création d'un Formulaire d'Inscription à une Newsletter

### Objectif :
Créer un composant Angular avec un formulaire permettant aux utilisateurs de s'inscrire à une newsletter. Le formulaire doit inclure les champs suivants :
- Nom
- Email

### Instructions :

1. **Créer le composant** :
   - Utilisez la CLI Angular pour générer un nouveau composant nommé `NewsletterSignup`.

2. **Configurer le FormGroup** :
   - Dans le fichier TypeScript du composant (`newsletter-signup.component.ts`), configurez un `FormGroup` avec deux `FormControl` pour les champs `name` et `email`.

3. **Template HTML** :
   - Créez le formulaire dans le fichier HTML du composant (`newsletter-signup.component.html`).
   - Utilisez `formGroup` pour lier le formulaire au `FormGroup` dans le fichier TypeScript.
   - Utilisez `formControlName` pour chaque champ du formulaire.

4. **Soumission du Formulaire** :
   - Implémentez une méthode `submitForm()` qui affiche les valeurs des champs dans la console.

5. **Gestion des Erreurs** ⭐️ :
   - Ajoutez des Validators pour les champs `name` (requis) et `email` (requis et format email valide).
   - Affichez des messages d'erreur conditionnels dans le template HTML pour informer l'utilisateur des erreurs de validation.



### Résultats Attendus :
- Un formulaire fonctionnel avec validation.
- Affichage de messages d'erreur lorsque les champs sont invalides.
- Affichage des données du formulaire dans la console lors de la soumission.
- ⭐️ Bonus : Gestion d'erreur avec affichage conditionnel des messages d'erreur.
