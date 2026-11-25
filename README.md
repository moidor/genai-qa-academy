# GenAI QA Academy · v2.0

PWA de préparation personnelle au CT-GenAI v1.1. 37 fiches, 300 questions d'entraînement, 40 questions de simulation (60 minutes, 46 points), flashcards et révisions. Application statique, sans compte ni API ; progression locale exportable en JSON.

## Démarrage

Ouvrir `index.html` pour les cours en local. Pour vérifier le service worker et le mode installable :

```sh
python -m http.server 8080
```

Ouvrir http://localhost:8080 dans Chrome ou Edge. Sur smartphone, utiliser l'URL HTTPS hébergée et le menu « Installer l’application » / « Ajouter à l’écran d’accueil ».

## GitHub Pages

Settings → Pages → Build and deployment → Source : Deploy from a branch → main / (root) → Save.
Consulter l'adresse affichée par GitHub après le déploiement (habituellement https://moidor.github.io/genai-qa-academy/).
Pour chaque mise à jour, modifier `content.js` (cours) / `bank.js` (questions, concepts, références) ou `app.js` (interface), et incrémenter `CACHE` dans `sw.js`.

## Sources et limites

Syllabus ISTQB® CT-GenAI v1.1 (27/04/2026), auteurs Abbas Ahmad, Gualtiero Bazzana, Alessandro Collino, Olivier Denoo, Bruno Legeard ; CFTL traduction française v1.0 ; Sample Exam A Questions et Answers v1.1, auteurs Abbas Ahmad, Alessandro Collino, Bruno Legeard. © ISTQB® et auteurs pour les sources. Support non officiel et non accrédité ; pas de redistribution des PDF ni de reproduction intégrale de l'examen. Vérifier les conditions de publication avant diffusion publique.

La banque comporte 254 variantes issues de 127 couples notion/exemple, 40 QCM de départ (dont une question à réponses multiples révisée), une seconde question multiple et 5 cas nouveaux. Les niveaux K sont les niveaux des objectifs associés, pas une validation indépendante de la difficulté de chaque item. Les 40 questions officielles sont indexées avec pages, points évalués et réponses ; lire les PDF d'origine à côté. La simulation utilise un tirage par objectif selon la distribution du Sample Exam A ; elle n'est pas un examen officiel. La progression est conservée par navigateur et par origine ; exporter/importer pour la transférer.

### En cas d'erreur 404

Vérifier que Pages utilise `main` et `/ (root)` et que le workflow `pages build and deployment` a réussi. Si aucune exécution n'apparaît, effectuer un commit depuis le compte propriétaire avec une adresse e-mail vérifiée.
