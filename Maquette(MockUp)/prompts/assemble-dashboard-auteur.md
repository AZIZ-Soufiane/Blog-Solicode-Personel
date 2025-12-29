# Prompt : Assemblage du Dashboard Auteur

Utilisez ce guide pour assembler ou reconstruire le Dashboard Auteur en utilisant les composants atomiques créés.

## 1. Structure de Base (index.html)
Commencez par un document HTML5 standard incluant les dépendances suivantes dans le `<head>` :
- Tailwind CSS via CDN.
- Lucide Icons via CDN.
- Google Fonts : `Inter` et `Outfit`.
- Configuration Tailwind spécifique (fonts: sans, heading; colors: primary).

## 2. Insertion des Composants (Ordre d'assemblage)
Assemblez les composants suivants dans cet ordre exact, en respectant la hiérarchie DOM de `dashboard-auteur.html` :

1.  **Sidebar :** Insérez le contenu de `components/layout/sidebar.html` au début du `<body>`.
2.  **Navbar :** Insérez le contenu de `components/layout/navbar.html`. Note : Le conteneur doit avoir la classe `lg:pl-64` pour l'alignement.
3.  **Conteneur Principal (`<main>`) :** Appliquez les classes `pt-10 px-4 sm:px-6 md:px-8 lg:pl-72`.
    -   **En-tête de section :** Ajoutez le titre "Dashboard Auteur" et le bouton "Nouvel Article".
    -   **KPIs Grid :** Insérez la grille de `components/data/kpi-card.html`.
    -   **Activité :** Insérez le widget de `components/widgets/recent-articles.html` sous les KPIs.

## 3. Scripts de Finalisation
Ajoutez ces scripts à la fin du `<body>` pour garantir l'interactivité :
- Preline JS (`preline.js`).
- Initialisation Lucide (`lucide.createIcons()`).
- Logique de Dropdown personnalisée pour le profil utilisateur.
