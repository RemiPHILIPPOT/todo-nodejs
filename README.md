# Application de gestion de tâches (ToDo App) en Node.js

Ce projet est une application de gestion de tâches simple développée en Node.js. Il permet aux utilisateurs de créer, lire, mettre à jour et supprimer des tâches.

## Fonctionnalités

-   **Authentification :** Les utilisateurs peuvent s'inscrire, se connecter et se déconnecter.
-   **Gestion des tâches :** Les utilisateurs peuvent créer, lire, mettre à jour et supprimer des tâches.
-   **Pagination :** La liste des tâches est paginée pour une meilleure expérience utilisateur.
-   **Tests unitaires :** Des tests unitaires sont inclus pour assurer la qualité du code.

## Installation

1. **Cloner le repository :**

```bash
    git clone https://github.com/votre-utilisateur/my-nodejs-project.git
```

2. **Installer les dépendances :**

```bash
cd my-nodejs-project
npm install
```

3. **Configurer la base de données :**

Modifier les paramètres de connexion à la base de données dans le fichier config/database.js.

4. **Démarrer le serveur :**

```bash
Copy code
npm start
```

Le serveur sera alors accessible à l'adresse http://localhost:3000.

## Utilisation

1. **S'inscrire :**

Envoyer une requête POST à http://localhost:3000/signup avec le corps suivant :

```json
{
    "username": "votre_nom_utilisateur",
    "password": "votre_mot_de_passe"
}
```

2. **Se connecter :**

Envoyer une requête POST à http://localhost:3000/login avec le corps suivant :

```json
{
    "username": "votre_nom_utilisateur",
    "password": "votre_mot_de_passe"
}
```

3. **Créer une tâche :**

Envoyer une requête POST à http://localhost:3000/tasks avec le corps suivant :

```json
{
    "title": "Titre de la tâche",
    "description": "Description de la tâche"
}
```

4. **Lire une tâche :**

Envoyer une requête GET à http://localhost:3000/tasks/:id où :id est l'identifiant de la tâche.

5. **Mettre à jour une tâche :**

Envoyer une requête PUT à http://localhost:3000/tasks/:id où `:id
