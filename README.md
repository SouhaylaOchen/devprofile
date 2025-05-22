# DevProfile – Application Web Laravel

**DevProfile** est une application web moderne développée avec **Laravel 11**, permettant aux développeurs de créer un profil personnel, de gérer leurs projets et compétences, et de générer un CV téléchargeable au format PDF. Ce projet a été réalisé dans le cadre du module *Développement Web Avancé* à l’École Supérieure de Technologie.
![image](https://github.com/user-attachments/assets/9c6e040a-b16c-4e8e-bdbf-c2f44bd2ad1a)
![image](https://github.com/user-attachments/assets/fa8a9699-2c29-4280-a911-6b8c5d3e3bf2)
![image](https://github.com/user-attachments/assets/bb3c6e9d-9876-4442-b1ef-7b9c1528b840)
![image](https://github.com/user-attachments/assets/f6558781-dfc8-4e0d-9c1c-e79dc2082854)
![image](https://github.com/user-attachments/assets/17301db1-981d-4ee3-9423-0864a56f9229)

---

##  Objectifs du projet

Ce projet vise à :

- Mettre en œuvre l'architecture MVC avec Laravel.
- Maîtriser la gestion des routes, des contrôleurs, et des vues avec Blade.
- Implémenter un système d’authentification sécurisé.
- Manipuler une base de données relationnelle avec Eloquent ORM.
- Générer dynamiquement des fichiers PDF avec les données utilisateur.
- Présenter une application fonctionnelle et professionnelle.

---

## Fonctionnalités principales

L’application comprend les modules suivants :

### Authentification
- Inscription, connexion, déconnexion via **Laravel Breeze**.
- Protection des routes par middleware `auth`.


### Profil utilisateur
- Modification des informations : nom, email, titre, biographie.
- URL publique de type `/profile/username`.
![Capture d'écran 2025-05-22 203203](https://github.com/user-attachments/assets/554505d4-7e59-4fb4-9351-66d588da9cc0)
![Capture d'écran 2025-05-22 203318](https://github.com/user-attachments/assets/e1195b61-f35a-4d59-98f4-79906a65a1c6)
![Capture d'écran 2025-05-22 203453](https://github.com/user-attachments/assets/c301acfb-6cf0-49fa-8b9d-b6efc8c0af56)
![Capture d'écran 2025-05-22 203515](https://github.com/user-attachments/assets/9575de66-4259-423f-b855-476ed0838665)
![Capture d'écran 2025-05-22 203537](https://github.com/user-attachments/assets/8001f286-97b0-4f10-bd73-638006350faf)



### Gestion des projets
- Ajout, modification, suppression de projets avec titre, description et lien.
- Affichage des projets sur la page de profil public.

![image](https://github.com/user-attachments/assets/35f01c75-e5fc-4e17-9183-f5bc23a58152)
![image](https://github.com/user-attachments/assets/ba847ab1-b784-43c6-abc3-b5c6d06e8422)

### Compétences
- Ajout et suppression de compétences (ex. : PHP, Laravel, JavaScript).
- Affichage sur le profil utilisateur.

![image](https://github.com/user-attachments/assets/2cac7704-a1a1-44d1-90b5-92035c9164c8)
![image](https://github.com/user-attachments/assets/be3c409e-8ada-417b-aafb-2af52780e742)

### Génération de CV PDF
- Bouton pour télécharger le CV généré dynamiquement avec les données du profil.
- Intégration avec DomPDF.

![image](https://github.com/user-attachments/assets/2d30c63a-ac6c-4197-9196-be10acdbad4f)
![image](https://github.com/user-attachments/assets/c2665ce0-e3fa-46e9-bd45-e2f416a858b4)

---

## Architecture technique

L'application suit l'architecture **MVC** :

- **Modèles** : User, Project, Skill
- **Contrôleurs** : ProfileController, ProjectController, SkillController, PDFController
- **Vues** : gérées avec Blade
- **Relations Eloquent** :
  - Un utilisateur possède plusieurs projets.
  - Un utilisateur possède plusieurs compétences.


---

##  Technologies utilisées

| Composant               | Détail                          |
|-------------------------|----------------------------------|
| Framework Backend       | Laravel 11                      |
| Authentification        | Laravel Breeze (stack Blade)    |
| Base de Données         | MySQL 8.x                       |
| Stylisation             | Tailwind CSS                    |
| Génération de PDF       | Laravel DomPDF                  |
| Gestion des Assets      | Node.js + NPM                   |

---

##  Installation locale

### Prérequis
- PHP >= 8.2
- MySQL
- Composer
- Node.js + npm

### Étapes

1. Cloner le projet :
```bash
git clone https://github.com/SouhaylaOchen/devprofile.git
cd devprofile
```

2. Installer les dépendances :
```bash
composer install
npm install
```

3. Configurer l'environnement :
```bash
cp .env.example .env
php artisan key:generate
```

4. Configurer la base de données dans le fichier `.env`.

5. Lancer les migrations :
```bash
php artisan migrate
```

6. Compiler les assets :
```bash
npm run build
```

7. Démarrer le serveur :
```bash
php artisan serve
```

---

##  Tests effectués

| Fonctionnalité        | Statut | Méthode                   |
|------------------------|--------|---------------------------|
| Authentification       | OK     | Formulaires Laravel Breeze|
| CRUD Projets           | OK     | Tests manuels             |
| Gestion des compétences| OK     | Ajout/Suppression         |
| Génération PDF         | OK     | Téléchargement fonctionnel|

---

##  Améliorations futures

Voici quelques pistes pour faire évoluer l’application :

- Ajouter une **prévisualisation** du CV.
- Permettre l’**upload d’une photo de profil**.
- Ajouter une **version mobile** ou une **PWA**.
- Ajouter la **prise en charge du multilingue** (FR/EN).
- Mettre en place des **rôles utilisateurs** (admin, visiteur, etc.).

---


##  Réalisé par

Projet académique réalisé dans le cadre de la formation :

*  1ère année — InGénierer Logiciel & Cybersécurité
*  Développé par : Souhayla Ouchen ET Oumaima Marzak  
*  Encadré par :RABHI Ouzayr 



