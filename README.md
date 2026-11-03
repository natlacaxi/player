# TalcoPlayer

Plateforme de jeux : **Undercover** et **Pendu**, ouverts en iframe. Installable comme application mobile (PWA).

## Mise en ligne (GitHub Pages)

1. Crée un dépôt (ex. `talcoplayer`) et envoie-y ces fichiers sur la branche `main`.
2. Dépôt → **Settings → Secrets and variables → Actions → New repository secret** :
   - `PLAYER_2` = `https://natlacaxi.github.io/undercover` (Undercover)
   - `PLAYER_1` = `https://natlacaxi.github.io/pendu` (Pendu)
3. Dépôt → **Settings → Pages → Source : GitHub Actions**.
4. Pousse sur `main` (ou lance le workflow à la main) : le site est publié.

Les liens ne sont pas dans le code du dépôt : le workflow remplace `__PLAYER_1__` et `__PLAYER_2__` dans `index.html` au déploiement.
Attention : sur un site statique, ils restent visibles dans le code servi au navigateur.

## À compléter
Les champs `[À COMPLÉTER]` des mentions légales dans `index.html`.

## Tester en local
Remplace `__PLAYER_2__` et `__PLAYER_1__` dans `index.html`, puis sers le dossier (`python3 -m http.server`).
