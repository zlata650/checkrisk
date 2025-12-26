# 🚀 Déploiement sur Netlify

## Méthode 1 : Glisser-Déposer (La plus simple)

1. Allez sur [netlify.com](https://www.netlify.com)
2. Créez un compte gratuit (ou connectez-vous)
3. Sur la page d'accueil, vous verrez une zone "Deploy manually"
4. **Glissez-déposez le dossier `CheckRisk`** dans cette zone
5. Netlify va automatiquement déployer votre site
6. Vous obtiendrez une URL comme : `https://votre-site-123.netlify.app`

## Méthode 2 : Via GitHub (Recommandé pour les mises à jour automatiques)

1. Allez sur [netlify.com](https://www.netlify.com)
2. Cliquez sur "Add new site" > "Import an existing project"
3. Sélectionnez "GitHub"
4. Autorisez Netlify à accéder à votre compte GitHub
5. Sélectionnez le dépôt `zlata650/checkrisk`
6. Configurez :
   - **Build command** : (laissez vide, pas de build nécessaire)
   - **Publish directory** : `/` (racine)
7. Cliquez sur "Deploy site"

**Avantage** : Chaque fois que vous poussez des changements sur GitHub, Netlify redéploiera automatiquement votre site !

## Méthode 3 : Via Netlify CLI (Pour les développeurs)

```bash
# Installer Netlify CLI
npm install -g netlify-cli

# Se connecter
netlify login

# Dans le dossier CheckRisk
cd /Users/zlatashvets/CheckRisk

# Déployer
netlify deploy --prod
```

## 🔗 Obtenir le lien de votre site

Une fois déployé, vous obtiendrez :
- Une URL automatique : `https://votre-site-123.netlify.app`
- Vous pouvez la personnaliser dans : Site settings > Domain management > Custom domain

## 📝 Mettre à jour le site

### Si vous avez utilisé GitHub :
```bash
git add .
git commit -m "Mise à jour"
git push
```
Netlify redéploiera automatiquement !

### Si vous avez utilisé glisser-déposer :
Glissez-déposez à nouveau le dossier mis à jour.

## ✅ Votre site est maintenant en ligne !

 Partagez le lien avec ChatGPT ou qui vous voulez !

