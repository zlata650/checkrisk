# Guide de déploiement - CheckRisk

## Option 1 : Netlify (Recommandé - Le plus simple)

1. Allez sur [netlify.com](https://netlify.com) et créez un compte (gratuit)
2. Glissez-déposez le dossier `CheckRisk` dans la zone de déploiement
3. Votre site sera en ligne en quelques secondes !
4. Vous obtiendrez une URL comme : `https://votre-site.netlify.app`

**Avantages :**
- Gratuit
- Déploiement en 1 clic
- HTTPS automatique
- URL personnalisée possible

## Option 2 : GitHub Pages

1. Créez un compte sur [github.com](https://github.com) si vous n'en avez pas
2. Créez un nouveau dépôt (repository)
3. Uploadez vos fichiers :
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/VOTRE-USERNAME/checkrisk.git
git push -u origin main
```
4. Allez dans Settings > Pages
5. Sélectionnez la branche `main` et le dossier `/ (root)`
6. Votre site sera disponible sur : `https://VOTRE-USERNAME.github.io/checkrisk`

## Option 3 : Vercel

1. Allez sur [vercel.com](https://vercel.com) et créez un compte
2. Installez Vercel CLI : `npm i -g vercel`
3. Dans le dossier CheckRisk, exécutez : `vercel`
4. Suivez les instructions
5. Votre site sera en ligne !

## Option 4 : Surge.sh (Simple et rapide)

1. Installez Surge : `npm install -g surge`
2. Dans le dossier CheckRisk, exécutez : `surge`
3. Suivez les instructions pour créer un compte
4. Votre site sera en ligne sur une URL comme : `https://votre-site.surge.sh`

---

**Note importante :** Le serveur proxy (simple-proxy.js) ne fonctionnera pas sur ces plateformes car elles servent uniquement des fichiers statiques. L'iframe chargera directement depuis `https://mammogene-frontend-fuld.onrender.com/`.

