# Kasa 🏠

Application web de location immobilière entre particuliers, développée dans le cadre du projet 5 de la formation Développeur Web OpenClassrooms.

![React](https://img.shields.io/badge/React-19-61DAFB?logo=react&logoColor=white)
![React Router](https://img.shields.io/badge/React_Router-7-CA4245?logo=reactrouter&logoColor=white)
![Sass](https://img.shields.io/badge/Sass-CC6699?logo=sass&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-7-646CFF?logo=vite&logoColor=white)

## 📋 Description

Kasa est une refonte front-end d'une application de location immobilière. Le projet consiste à créer l'intégralité de l'interface React à partir de maquettes Figma, en utilisant des données JSON statiques.

**Fonctionnalités :**
- Affichage de la liste des logements disponibles
- Page de détail d'un logement (galerie photos, description, équipements, règles)
- Composant Slideshow (carousel) pour les photos
- Composant Collapse (accordéon) pour les informations dépliables
- Page À propos
- Page 404 personnalisée pour les routes inconnues

## 🛠️ Stack technique

| Technologie | Version | Usage |
|---|---|---|
| React | 19 | Framework UI |
| React Router DOM | 7 | Gestion des routes |
| Sass | 1.97 | Styles CSS (architecture 7-1 partielle) |
| Vite | 7 | Bundler & serveur de développement |

## 🚀 Installation et lancement

### Prérequis

- Node.js ≥ 18
- npm ≥ 9

### Étapes

```bash
# 1. Cloner le dépôt
git clone https://github.com/AuguiMaxime/Kasa.git
cd Kasa

# 2. Installer les dépendances
npm install

# 3. Lancer le serveur de développement
npm run dev
```

L'application est accessible à l'adresse : `http://localhost:5173`

### Scripts disponibles

```bash
npm run dev       # Lance le serveur de développement
npm run build     # Génère le build de production dans /dist
npm run preview   # Prévisualise le build de production
npm run lint      # Analyse le code avec ESLint
```

## 📁 Structure du projet

```
Kasa/
├── index.html
├── package.json
├── vite.config.js
└── src/
    ├── main.jsx              # Point d'entrée React
    ├── App.jsx               # Composant racine
    ├── router/
    │   └── Router.jsx        # Définition des routes
    ├── pages/
    │   ├── Layout.jsx        # Layout partagé (Header + Footer)
    │   ├── Home.jsx          # Page d'accueil
    │   ├── About.jsx         # Page À propos
    │   ├── Logement.jsx      # Page détail d'un logement
    │   └── Notfound.jsx      # Page 404
    ├── components/
    │   ├── Header.jsx
    │   ├── Footer.jsx
    │   ├── Card.jsx          # Carte d'un logement (liste)
    │   ├── Slideshow.jsx     # Carrousel de photos
    │   ├── Collapse.jsx      # Accordéon générique
    │   ├── CollapseAbout.jsx # Accordéon page About
    │   ├── Gallery.jsx       # Galerie de la page Home
    │   ├── LogementContent.jsx
    │   ├── BannerHome.jsx
    │   ├── BannerAbout.jsx
    │   └── Assets/           # Images et icônes statiques
    ├── data/
    │   └── logements.json    # Données statiques des logements
    └── styles/
        ├── base/
        │   ├── _global.scss
        │   └── _variables.scss
        └── components/       # Styles Sass par composant
```

## 🌐 Démo

 🔗 [Voir la démo en ligne](https://kasa-green-xi.vercel.app)

## 📝 Notes de développement

- Les données sont issues d'un fichier JSON statique (`logements.json`) — aucune API back-end n'est utilisée
- La navigation vers une URL `/logement/:id` inexistante redirige vers la page 404
- L'architecture Sass suit une approche par composant (un fichier `_composant.scss` par composant)

## 👨‍💻 Auteur

**Maxime Augui** — Développeur Web Full-Stack  
[Portfolio](https://portfolio-sigma-bay-72.vercel.app) · [GitHub](https://github.com/AuguiMaxime)
