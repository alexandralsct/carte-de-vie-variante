# Chantier « moteur » (branche chantier-moteur, rien fusionné dans main)

Objectif : variante aussi interactive que la carte (espaces, onglets, recettes, items, Omniscient), sans contenu privé ni clé dans ce dépôt public.

## État
- Étape 1 faite : menu ⋯ → « Vraie carte » = la carte réelle en plein écran sous l'en-tête (iframe ../carte-de-vie/, même origine, déjà connectée, charge elle-même son module privé). V.0.0.22, cache carte-life-v25.
- Vérifié : Playwright 412 px, aucune erreur JS, aucun débordement, carte vide (sans données).
- Non vérifié (données privées + clé requises, GitHub Pages inaccessible depuis le conteneur) : clics sur espaces/onglets/recettes/items, Omniscient, chargement du module privé. À tester en ligne après déploiement.

## Suite possible
- Étape 2 : ouvrir la vraie carte directement sur l'espace choisi, ou porter le moteur (CROCHETS, Object.assign) dans la variante.
- Règles : petites étapes, version + cache sw.js incrémentés, capture 412 px, test Playwright, push après chaque étape, pas de PR ni de fusion sans accord.
