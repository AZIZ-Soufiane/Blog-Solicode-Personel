# 📄 Spécifications : Dashboard Auteur (Light Mode)

**Maquette Cible :** `dashboard-auteur.html`
**Rôle :** Auteur - Accès restreint au contenu personnel.

---

## 1. Structure de la Page (Layout)
Le dashboard est composé de trois zones principales gérées par des composants dédiés :

*   **Sidebar :** [sidebar.html](file:///c:/GitHub/Blog-Solicode-Personel/Maquette%28MockUp%29/components/layout/sidebar.html) - Navigation restreinte au Dashboard uniquement.
*   **Navbar :** [navbar.html](file:///c:/GitHub/Blog-Solicode-Personel/Maquette%28MockUp%29/components/layout/navbar.html) - En-tête avec profil utilisateur (Sarah Auteur) et lien de déconnexion.
*   **Main Content :** Zone centrale incluant le titre, le bouton "Nouvel Article", les KPIs et l'activité.

---

## 2. Indicateurs de Performance (KPIs)
Composant : [kpi-card.html](file:///c:/GitHub/Blog-Solicode-Personel/Maquette%28MockUp%29/components/data/kpi-card.html)

Affiche les statistiques personnelles de l'auteur :
*   **Mes Articles :** Nombre total d'articles créés par l'utilisateur.
*   **Total Vues :** Somme des vues sur l'ensemble de ses publications.

---

## 3. Widget d'Activité
Composant : [recent-articles.html](file:///c:/GitHub/Blog-Solicode-Personel/Maquette%28MockUp%29/components/widgets/recent-articles.html)

Remplace la liste des articles par un flux d'activité chronologique ("Votre Activité") montrant :
*   Les sauvegardes de brouillons.
*   Les validations d'articles par l'administration.

---

## 4. Design & Thème
*   **Mode :** Light Mode exclusif (classes `dark:` supprimées des composants).
*   **Typographie :** `Inter` (corps) et `Outfit` (titres).
*   **Couleurs :** Palette Blue/Gray épurée.