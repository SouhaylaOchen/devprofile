![image](https://github.com/user-attachments/assets/6fc73539-fcad-496a-b00c-b1a467e4229f)


````markdown
# DevProfile – Application Laravel

DevProfile est une application web développée avec Laravel, conçue pour permettre aux développeurs de créer un profil professionnel en ligne, de gérer leurs projets et compétences, et de générer un CV en format PDF. Ce projet a été réalisé dans le cadre du module **Développement Web Avancé**.

## 🚀 Objectifs du projet

- Créer une application Laravel fonctionnelle en respectant l'architecture MVC.
- Implémenter un système complet d’authentification.
- Gérer dynamiquement des données utilisateurs (projets et compétences).
- Générer un CV à partir des données saisies.
- Structurer un projet web moderne prêt à être déployé.

## 🔧 Fonctionnalités principales

- Inscription, connexion et déconnexion via Laravel Breeze.
- Modification du profil utilisateur (nom, titre, bio, email...).
- CRUD complet des projets (titre, description, lien).
- Ajout et suppression de compétences.
- Génération automatique d’un fichier CV au format PDF.
- Affichage d’un profil public via une URL unique (`/profile/username`).

## 🧱 Architecture du projet

L’application suit le modèle **MVC** (Modèle - Vue - Contrôleur) :

- **Modèles** : User, Project, Skill
- **Vues** : Blade templates
- **Contrôleurs** : ProfileController, ProjectController, SkillController, PDFController
- **Relations Eloquent** :
  - Un utilisateur possède plusieurs projets
  - Un utilisateur possède plusieurs compétences

## 📂 Technologies utilisées

- Laravel 11
- Laravel Breeze (authentification)
- PHP 8.2+
- MySQL
- Tailwind CSS
- DomPDF (pour la génération PDF)
- Git & GitHub

## 🖥️ Aperçu de l'application

> Veuillez insérer ici des captures d’écran de l’application (page de profil, gestion des projets, aperçu du CV PDF, etc.)

## ▶️ Installation locale

### Prérequis

- PHP >= 8.2
- Composer
- MySQL
- Node.js & npm

### Étapes

1. Cloner le dépôt :
   ```bash
   git clone https://github.com/votre-utilisateur/devprofile.git
   cd devprofile
````

2. Installer les dépendances PHP et JS :

   ```bash
   composer install
   npm install && npm run dev
   ```

3. Configurer le fichier `.env` :

   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. Créer la base de données MySQL et configurer l’accès dans `.env`.

5. Lancer les migrations :

   ```bash
   php artisan migrate
   ```

6. Lancer le serveur :

   ```bash
   php artisan serve
   ```

7. Accéder à l’application via `http://localhost:8000`.

## 🧪 Tests manuels réalisés

* Authentification (inscription/connexion)
* Gestion de profil
* CRUD projets et compétences
* Affichage du profil public
* Génération du PDF

## 📈 Améliorations futures

* Ajout d’une prévisualisation du CV avant génération.
* Upload d’image de profil.
* Version multilingue (FR/EN).
* Version mobile ou PWA.
* Gestion des rôles utilisateurs (admin, visiteur...).

## 📬 Contribution

Ce projet a été réalisé par Souhayla Ouchen dans un cadre académique. Toute contribution ou suggestion est la bienvenue.

---

Merci pour votre intérêt pour DevProfile !

```

---

```
