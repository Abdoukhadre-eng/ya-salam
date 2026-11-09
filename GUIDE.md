# Ya Salam — mise en ligne

Conçu et développé par Abdoukhadre Boye

## 1. Préparer la liste des vidéos (Google Sheet)

1. Créer un Google Sheet, renommer l'onglet **Videos**.
2. Mettre ces en-têtes en ligne 1 (voir `modele-sheet.csv`) :
   `Titre | Témoin | Catégorie | Date | Lien | Vignette`
3. Une ligne = une vidéo. Seuls **Titre** et **Lien** sont obligatoires.
   - Date au format `2026-11-09` (les plus récentes s'affichent en premier).
   - Catégorie : Miracles, Vécu, Enseignements… — chaque catégorie devient un filtre.
   - Vignette : lien d'une image (facultatif ; YouTube et Drive en ont une automatiquement).
4. **Partager** → « Tous les utilisateurs disposant du lien » → **Lecteur**.
5. Copier l'identifiant du Sheet : la partie entre `/d/` et `/edit` dans le lien.

## 2. Liens acceptés dans la colonne « Lien »

| Source | Lecture dans l'app | Téléchargement |
|---|---|---|
| TikTok (lien complet `…/video/123…`) | Oui | Via l'app TikTok (si le créateur l'autorise) |
| Google Drive (fichier partagé « Lecteur ») | Oui | **Oui, bouton direct** |
| YouTube | Oui | Non |
| Fichier `.mp4` en ligne | Oui | Oui |

Les liens TikTok courts (`vm.tiktok.com/…`) ne se lisent pas dans l'app : ouvrir le lien
dans un navigateur et copier le lien complet qui s'affiche.

👉 Pour que les gens puissent **télécharger**, mettre les vidéos sur Google Drive.
Attention : Drive affiche un avertissement pour les fichiers de plus de ~100 Mo.

## 3. Brancher le Sheet

Ouvrir `index.html`, chercher `const SHEET_ID = "";` et coller l'identifiant entre les guillemets.

## 4. Publier sur GitHub Pages (comme Robinet Bi)

1. Créer un dépôt public, par ex. `ya-salam`.
2. Y déposer tous les fichiers du dossier (index.html, manifest.json, sw.js, dossier icons).
3. Settings → Pages → Branch `main` / `root` → Save.
4. Le lien sera : `https://<ton-compte>.github.io/ya-salam/`

## 5. Installer sur téléphone

- Android (Chrome) : bouton **Installer** dans l'app, ou menu ⋮ → « Ajouter à l'écran d'accueil ».
- iPhone (Safari) : Partager → « Sur l'écran d'accueil ».

## Ajouter une vidéo ensuite

Ajouter une ligne dans le Sheet — l'app se met à jour toute seule, sans republier.
