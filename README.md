# CUT 31 — PWA iPhone

Mini-app web installable sur l’écran d’accueil pour suivre un programme de 31 jours du 25 août au 24 septembre 2026.

## Fonctionnalités

- Jour affiché automatiquement selon la date du téléphone
- 31 journées complètes intégrées dans l’app
- Repas avec quantités, sans petit-déjeuner imposé
- Exercices, séries, répétitions, cardio et objectif de pas
- Hydratation par paliers jusqu’à 3 L
- Pesée et sommeil quotidiens
- Cases à cocher persistantes
- Streak et progression globale
- Courbe de poids
- Pensée stoïcienne, mission et visualisation quotidiennes
- Notes / victoire du jour
- Export / import JSON
- Fonctionnement hors ligne après la première ouverture
- Pas de compte ni de base de données : données stockées localement sur l’iPhone

## Installation iPhone

1. Ouvrir l’URL de l’app dans Safari.
2. Toucher **Partager**.
3. Choisir **Ajouter à l’écran d’accueil**.
4. Activer **Ouvrir comme app** si l’option apparaît.
5. Ajouter.

## Déploiement

L’app est statique et n’a aucune étape de build. Elle peut être hébergée sur Vercel ou GitHub Pages. Un workflow GitHub Pages est fourni dans `.github/workflows/pages.yml`.

Pour un dépôt privé, Vercel est généralement le chemin le plus simple si GitHub Pages n’est pas disponible sur le plan GitHub utilisé.

## Données

Les données sont stockées dans `localStorage` sous la clé `cut31-v2`. Utiliser **Réglages → Exporter mes données** pour conserver une sauvegarde portable.

## Développement local

```bash
python3 -m http.server 8080
```

Puis ouvrir `http://localhost:8080`.
