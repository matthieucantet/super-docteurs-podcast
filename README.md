# Super Docteurs

Site du podcast Super Docteurs, construit avec Astro.

## Développement

```sh
npm install
npm run dev
```

Le site local est disponible sur `http://localhost:4321`.

## Production

```sh
npm run build
```

Astro génère le site statique dans `dist/`.

## Déploiement Cloudflare Pages

1. Crée un dépôt GitHub vide nommé `super-docteurs-podcast`.
2. Ajoute ce dépôt comme remote puis envoie la branche principale :

```sh
git remote add origin https://github.com/VOTRE_COMPTE/super-docteurs-podcast.git
git branch -M main
git add .
git commit -m "Initialise le site Super Docteurs"
git push -u origin main
```

3. Dans Cloudflare, ouvre **Workers & Pages**, puis **Create application** et **Pages**.
4. Connecte le dépôt GitHub `super-docteurs-podcast`.
5. Utilise ces réglages :

| Réglage | Valeur |
| --- | --- |
| Framework preset | Astro |
| Build command | `npm run build` |
| Build output directory | `dist` |
| Node.js version | `22` |

Cloudflare Pages créera un déploiement de production à chaque push sur `main` et une URL de prévisualisation pour chaque pull request.
