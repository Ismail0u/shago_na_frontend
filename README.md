## README pour le Dépôt Frontend (Web & Mobile)

###  Plateforme SaaS de Gestion Commerciale - Frontend & Mobile

Ce dépôt regroupe les clients de l'API : l'application **Web (React)** pour les opérations avancées/administration et l'application **Mobile (Flutter)** pour la gestion rapide des ventes/stocks et le mode hors ligne.

-----

###  Application Web (React)

Utilisée par les **Administrateurs** (interface complète) et les **Commerçants** (opérations avancées, rapports). 

  * **Framework/Lib:** React + Vite 
  * **Gestion d'État:** Redux Toolkit / Zustand 
  * **API Calls:** Axios 
  * **UI/Design:** TailwindCSS + Shadcn/ui (et potentiellement Chakra) 
  * **Charts:** Recharts 
  * **Fonctionnalités Clés:** Tableau de bord avancé, gestion des abonnements, back-office d'administration, exportation de données (CSV/PDF). 

-----

### Application Mobile (Flutter)

Utilisée principalement par les **Vendeurs** et les **Commerçants** pour les transactions rapides et le travail **hors ligne**.

  * **Framework:** Flutter 3.24+ 
  * **Gestion d'État:** Riverpod 
  * **Stockage Local (Offline):** Drift / Hive 
  * **Navigation:** AutoRoute 
  * **Synchronisation:** Support de la synchronisation hors ligne $\rightarrow$ en ligne (via un service en arrière-plan toutes les 5 min). 
  * **Plateformes:** Support initial pour **Android 10+** (iOS ultérieurement). 

-----

### Démarrage Local

#### 1\. Configuration (Commune)

Assurez-vous que le **Backend** est opérationnel et notez son URL.

#### 2\. Application Web (React)

1.  **Installer les dépendances:**
    ```bash
    cd web
    npm install
    ```
2.  **Lancer le serveur de développement:**
    ```bash
    npm run dev
    ```
3.  Accédez à l'application web sur l'adresse fournie par Vite (généralement `http://localhost:5173`).

#### 3\. Application Mobile (Flutter)

1.  **Installer les dépendances:**
    ```bash
    cd mobile
    flutter pub get
    ```
2.  **Lancer l'application** (sur émulateur ou appareil Android) :
    ```bash
    flutter run
    ```
3.  Pour les tests de la fonctionnalité **hors ligne**, assurez-vous de configurer correctement les services de stockage local. 

-----

