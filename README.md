# Écho

Écho transforme tes cours en fiches réflexes, en jeux et en points.
On photographie, écrit ou colle un cours, et l'appli en tire des fiches, des cartes à retourner, des jeux, un parcours avec grades et un diplôme.

## Ce qu'il y a dans ce dossier

| Fichier | À quoi il sert |
|---|---|
| `index.html` | Toute l'appli (un seul fichier) |
| `manifest.webmanifest` | Nom, couleurs et icônes quand on l'installe sur l'écran d'accueil |
| `sw.js` | Permet à l'appli de s'ouvrir même sans internet |
| `apple-touch-icon.png` | Icône sur l'écran d'accueil de l'iPhone |
| `icon-192.png`, `icon-512.png` | Icônes pour Android et le navigateur |
| `icon-1024.png`, `icon.svg` | Logo en grand, pour un futur App Store ou une présentation |
| `README.md` | Ce guide |

Tous les fichiers doivent rester ensemble, à la racine du dépôt (pas dans un sous-dossier).

## Mettre l'appli en ligne avec GitHub Pages

Pas besoin d'installer quoi que ce soit : tout se fait sur le site de GitHub.

1. **Crée le dépôt.** Sur github.com, clique sur **+** en haut à droite, puis **New repository**.
   - Nom : `echo`
   - Coche **Public** (GitHub Pages gratuit demande un dépôt public ; seul le code est visible, jamais les cours ni les points des utilisateurs, qui restent sur leur téléphone).
   - Clique sur **Create repository**.
2. **Envoie les fichiers.** Sur la page du dépôt, clique sur **uploading an existing file** (ou **Add file → Upload files**).
   Glisse tous les fichiers du dossier (pas le dossier lui-même), puis clique sur **Commit changes**.
3. **Active GitHub Pages.** Va dans **Settings → Pages**.
   - Source : **Deploy from a branch**
   - Branch : **main**, dossier **/ (root)**, puis **Save**.
4. **Attends 1 à 2 minutes.** L'adresse apparaît en haut de la page Pages :
   `https://TON-PSEUDO.github.io/echo/`

## L'installer sur iPhone

1. Ouvre l'adresse dans **Safari**.
2. Touche le bouton **Partager** (le carré avec la flèche).
3. Choisis **Sur l'écran d'accueil**, puis **Ajouter**.

L'icône Écho apparaît comme une vraie appli et s'ouvre en plein écran.
Sur Android, Chrome propose **Installer l'application** dans son menu.

## Mettre à jour l'appli

1. Dans le dépôt, **Add file → Upload files**, glisse le nouveau `index.html` (il remplace l'ancien), puis **Commit changes**.
2. Attends 1 à 2 minutes, puis ferme et rouvre l'appli sur le téléphone.
3. Si le téléphone montre encore l'ancienne version, ouvre `sw.js` dans GitHub (crayon pour modifier), change `echo-v1` en `echo-v2`, puis **Commit changes**.

## À savoir

- **Les données restent sur chaque téléphone** (cours, points, grades). Rien n'est envoyé sur internet.
  Pour changer de téléphone : **Mon bureau → Exporter mes données**, puis **Importer** sur le nouveau.
- **Effacer les données de Safari efface aussi les cours.** Pense à exporter de temps en temps.
- **La lecture des photos** a besoin d'internet la première fois, pour télécharger le lecteur de texte en français (quelques Mo). Ensuite, tout le reste marche hors ligne.
- **Partager avec des collègues** : envoie-leur simplement l'adresse. Chacun a ses propres cours et ses propres points.
