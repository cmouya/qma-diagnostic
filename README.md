# QMA Diagnostic — Application PWA (v3)

Application mobile-first d'assistance aux candidats du concours de bourses d'excellence
« Québec Métiers d'Avenir » 2026-2027 (formation professionnelle, MEQ).
Centralisation des résultats : **cmouya@congobourse.org** · WhatsApp conseiller : **+243 84 892 453**

## Fichiers
- `index.html` — application complète (aucune dépendance)
- `manifest.json`, `sw.js` — PWA (installation + hors ligne)
- `news.json` — **nouvelles publiées par le conseiller** (modifiez ce fichier sur GitHub pour annoncer ateliers/rappels)
- `icon-*.png` — icônes

## Nouveautés v3
- 📤 Transmission centralisée du bilan : e-mail automatique (FormSubmit → cmouya@congobourse.org), WhatsApp (+243 84 892 453), e-mail classique — avec consentement et coordonnées candidat
- 👤 Mode conseiller multi-candidats : profils sauvegardés, export/import JSON
- 📰 Section « Nouvelles » alimentée par `news.json`
- ❓ FAQ trilingue intégrée (FR/EN/ES)
- 🌍 Interface FR / EN / ES
- 🌙 Mode sombre
- 🔔 Rappels d'échéances (notifications à l'ouverture, J-14)
- 📄 Export PDF via impression · ⬇️ export .txt
- 🔗 Liens officiels cliquables

## Publication des nouvelles (conseiller)
1. Ouvrez `news.json` sur GitHub → crayon ✏️
2. Ajoutez un objet `{"date":"AAAA-MM-JJ","titre":"…","texte":"…"}` en haut de la liste
3. « Commit changes » — visible par tous les candidats au prochain chargement (même hors ligne ensuite)

## ⚠️ Activation FormSubmit (une seule fois)
Le premier envoi depuis l'app déclenche un e-mail d'activation à **cmouya@congobourse.org**.
Cliquez le lien de confirmation dedans — les envois suivants arriveront directement.

## Déploiement
Hébergez tous les fichiers sur un serveur HTTPS (GitHub Pages : déjà en place chez vous).
Mettre à jour : remplacez `index.html`, `sw.js`, `manifest.json`, `news.json` sur GitHub (drag & drop ou commit).

## Confidentialité
Données stockées localement sur l'appareil du candidat (localStorage).
Transmission uniquement après consentement explicite, au conseiller désigné.
