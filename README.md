# QMA Diagnostic — Application PWA

Application mobile-first d'assistance aux candidats du concours de bourses d'excellence
« Québec Métiers d'Avenir » 2026-2027 (formation professionnelle, MEQ).

## Fichiers
- `index.html` — application complète (HTML/CSS/JS, aucune dépendance)
- `manifest.json` — manifeste PWA (installation sur l'écran d'accueil)
- `sw.js` — service worker (fonctionnement hors ligne)

## Déploiement
Hébergez les 3 fichiers sur n'importe quel serveur HTTPS (GitHub Pages, Netlify, Vercel…).
Ouvrez l'URL sur mobile → « Ajouter à l'écran d'accueil » pour l'installer comme application.

## Version 2 (tests terrain)
- 🧪 Mode démonstration (dossier exemple soins infirmiers) : chargé depuis le bilan, étape 5
- 🔄 Réinitialisation « Nouveau candidat » (efface le localStorage)
- 🔢 Compteurs de mots sur motivations (cible 150+) et parcours (cible 120+)
- 📋 Liste de vérification officielle (Annexe 4) affichée dans le bilan
- 🖨️ Feuille de style d'impression propre
- 🎨 Icônes PNG 192/512 + maskable (installabilité PWA complète)

## Fonctionnalités
1. **Diagnostic d'éligibilité** — questionnaire à branchement basé sur les 9 conditions du guide,
   verdict immédiat avec blocages identifiés.
2. **Projet d'études** — 18 formations priorisées offertes en français (Annexe 1, colonne « Oui »),
   régions priorisées signalées (≥ 50 % des bourses).
3. **Pièces du dossier** — checklist interactive des documents obligatoires + option langue + déclaration financière.
4. **Qualité de la candidature** — rédaction guidée selon la grille officielle (motivations 30 %, parcours 30 %…).
5. **Bilan** — score de complétion, pièces manquantes, export .txt / impression, calendrier du concours.

Données sauvegardées localement (localStorage) — aucune information transmise.
