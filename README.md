# 🛡️ SECURA - Plateforme de Sécurisation et de Gestion d'Événements

> **SECURA** révolutionne le contrôle d'accès aux événements au Cameroun et en Afrique Centrale. Notre solution web et mobile élimine les risques d'intrusion et de fraude documentaire en utilisant des **QR codes cryptés infalsifiables** pour garantir un accès exclusif aux invités légitimes.

## 🎯 Problématique et Solution

### Problématique
Les organisateurs d'événements au Cameroun (conférences, mariages haut de gamme, galas d'entreprise) font face à :
* La **fraude** et la duplication facile des invitations papier.
* Des **risques sécuritaires** importants lors du contrôle d'accès.
* Une **gestion logistique** manuelle et obsolète.

### Solution Proposée
**SECURA** est une plateforme intégrée qui offre :
1.  **Sécurité Renforcée :** Génération et envoi d'invitations numériques avec QR codes uniques, horodatés et cryptés.
2.  **Gestion Complète :** Tableau de bord pour l'organisation, l'import des listes d'invités, le design et l'envoi multi-canal (Email, SMS, WhatsApp).
3.  **Contrôle Fiable :** Application mobile de scan pour les agents d'accueil, avec validation instantanée et mode de **fonctionnement hors-ligne** (résilience technique).

---

## 🛠️ Stack Technique

Le projet est construit en adoptant une architecture moderne, performante et résiliente, adaptée aux défis de connectivité en Afrique.

| Composant | Technologie | Rôle / Justification |
| :--- | :--- | :--- |
| **Backend API** | **Laravel (PHP)** | Robustesse, rapidité de développement, sécurité et gestion des modèles complexes. |
| **Base de Données** | **Firebase** | Base de données NoSQL flexible, haute disponibilité et synchronisation rapide, idéale pour le temps réel. |
| **Frontend (Web)** | **Vue.js / Blade (Laravel)** | Interface organisateur complète, responsive design. |
| **Application Mobile** | **PWA (Progressive Web App)** | Permet le mode hors-ligne pour les agents de terrain et assure une compatibilité étendue sur divers terminaux Android/iOS. |
| **Sécurité** | **HTTPS / QR Codes Cryptés** | Protection des données en transit et validation infalsifiable des accès. |

---

## 🚀 Fonctionnalités Clés du MVP (Minimum Viable Product)

Le déploiement initial se concentrera sur les fonctionnalités essentielles pour valider le marché :

1.  **Espace Organisateur (Web)**
    * Création d'événements simplifiée (titre, date, lieu).
    * Import d'invités via fichier CSV/Excel.
    * Génération automatique des QR codes sécurisés.
    * Envoi des invitations par Email et lien WhatsApp.
2.  **Application Agent (Mobile)**
    * Scanner de QR code haute performance.
    * Validation instantanée de l'invité (statut, nom, photo).
    * Mode **Déconnecté** pour les zones sans réseau (synchronisation différée).
3.  **Logistique et Suivi**
    * Tableau de bord de suivi en temps réel des arrivées (Check-in/Check-out).

---

## 💻 Guide de Démarrage Local

Pour configurer et exécuter le projet SECURA sur votre machine locale, suivez ces étapes.

### Prérequis

* PHP (version compatible Laravel)
* Composer
* Node.js et npm
* Git
* Accès à un projet Firebase pour la base de données.

### Installation

1.  **Clonage du Dépôt (via SSH) :**
    ```bash
    git clone git@github.com:nigninguioadeline/SECURA-Platform.git
    cd SECURA-Platform
    ```

2.  **Configuration Backend (Laravel) :**
    ```bash
    composer install
    cp .env.example .env
    php artisan key:generate
    ```
    *Modifiez le fichier `.env` pour y ajouter vos identifiants de connexion **Firebase** et d'autres paramètres.*

3.  **Installation Frontend (Assets) :**
    ```bash
    npm install
    npm run dev
    # ou 'npm run watch' pour le développement continu
    ```

4.  **Démarrage du Serveur Local :**
    ```bash
    php artisan serve
    ```
    Le projet sera accessible localement (généralement sur `http://127.0.0.1:8000`).

---

## 🤝 Contribution


### **Identité de l'Auteur :**
* **nigninguioadeline@gmail.com** (via le compte GitHub actuel)