# GreenLeaf World 3.1 — Pack de quêtes, niveaux 1 à 10

Contenu du ZIP :
- `data/quetes_niveaux_1_10.json` : 30 quêtes (10 principales, 10 secondaires, 10 exploration) et une saga légendaire.
- `data/inventaire_quetes.csv` : inventaire compact des quêtes.
- `js/quests.js` : module d'affichage autonome exposant `window.GreenLeafQuests.render()`.
- `docs/INTEGRATION.md` : intégration prudente.
- `docs/TESTS_MANUELS.md` : liste de tests.
- `docs/PROGRESSION_ET_RECOMPENSES.md` : règles à confirmer.

Ceci est un pack d'ajout, pas une copie complète de l'application. Il ne remplace pas `index.html`, `app.js`, `auth.js` ou `characters.js`. Le module affiche les fiches mais n'accorde pas d'XP et ne valide pas les quêtes. Les XP et objets sont des propositions à comparer aux règles déjà présentes. Toute progression réelle doit être vérifiée côté serveur.
