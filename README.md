# 💼 DevProfile — Application Laravel de gestion de profils développeurs

DevProfile est une application web développée avec Laravel 12, conçue pour permettre aux développeurs de créer, gérer et partager leur profil professionnel, leurs projets et leurs compétences. Elle permet également de générer automatiquement un CV en PDF basé sur les informations du profil.

---

## 🖥️ Fonctionnalités principales

- Authentification avec Laravel Breeze
- Édition du profil utilisateur (nom, email, username, titre, biographie)
- Ajout, modification et suppression de projets
- Ajout et suppression de compétences
- Affichage public du profil via `/profile/{username}`
- Téléchargement du profil au format PDF
- Interface responsive et propre avec Tailwind CSS

---

## 🚀 Technologies utilisées

- PHP 8.2
- Laravel 12
- Laravel Breeze (Blade)
- Tailwind CSS
- MySQL / MariaDB
- Vite (pour les assets)
- DomPDF (pour la génération du PDF)

---

## ⚙️ Installation et configuration

1. Cloner ou copier le projet :

```bash
git clone https://votre-repo-github.com/username/devprofile.git
cd devprofile
````

2. Installer les dépendances :

```bash
composer install
npm install && npm run dev
```

3. Copier le fichier `.env` et générer la clé :

```bash
cp .env.example .env
php artisan key:generate
```

4. Configurer la base de données dans le fichier `.env` :

```
DB_DATABASE=devprofile
DB_USERNAME=root
DB_PASSWORD=...
```

5. Lancer les migrations :

```bash
php artisan migrate
```

6. Démarrer le serveur :

```bash
php artisan serve
```

Accéder à l’application : [http://127.0.0.1:8000](http://127.0.0.1:8000)

---

## 🧪 Navigation & Pages

* Tableau de bord : `/dashboard`
* Profil utilisateur : `/profile`
* Liste des projets : `/projects`
* Liste des compétences : `/skills`
* Profil public : `/profile/{username}`
* Génération PDF : `/pdf/{username}`

---

## 📂 Structure du projet

* `routes/web.php` : routes principales
* `app/Http/Controllers` : contrôleurs Laravel
* `resources/views` : interfaces utilisateur (Blade)
* `database/migrations` : création des tables

---

## 🔐 Sécurité

* Les routes sont protégées par le middleware `auth`
* Les utilisateurs non connectés sont redirigés vers `/login`
* Chaque utilisateur ne peut voir ou modifier que ses propres données

---

## 📄 Génération de CV en PDF

Le fichier PDF est généré automatiquement à partir de la vue :

```
resources/views/pdf/cv.blade.php
```

Accessible via : `/pdf/{username}`

---

## 🧑‍💻 Réalisé par

Projet académique réalisé dans le cadre de la formation :

* 🎓 1ère année — InGénierer Logiciel & Cybersécurité
* 👤 Développé par : \[Souhayla Ouchen et Oumayma Marzak]
* 🧑‍🏫 Encadré par : \[RABHI Ouzayr 
]

---

## ✅ État du projet

✔️ Finalisé et testé
📄 Rapport disponible séparément
📦 Prêt à être déployé ou livré

---
