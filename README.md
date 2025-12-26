# CheckRisk

Site web de présentation pour CheckRisk - Assistant IA pour l'évaluation du risque de cancer du sein.

## 🚀 Déploiement rapide

### Option la plus simple : Netlify

1. Allez sur [netlify.com](https://netlify.com)
2. Créez un compte (gratuit)
3. Glissez-déposez le dossier dans la zone de déploiement
4. Votre site est en ligne !

### Autres options

Voir [DEPLOY.md](DEPLOY.md) pour d'autres méthodes de déploiement (GitHub Pages, Vercel, Surge.sh).

## 📁 Structure

- `index.html` - Page principale du site
- `simple-proxy.js` - Serveur proxy local (pour développement)
- `package.json` - Dépendances Node.js

## 🛠️ Développement local

Pour tester localement avec le proxy :

```bash
npm install
npm start
```

Puis ouvrez `index.html` dans votre navigateur ou utilisez un serveur HTTP local :

```bash
python3 -m http.server 8000
```

Accédez à http://localhost:8000

## 📝 Notes

- Le site est entièrement statique (HTML/CSS/JavaScript)
- L'iframe dans la section démo charge directement depuis `https://mammogene-frontend-fuld.onrender.com/`
- Le proxy local (`simple-proxy.js`) n'est nécessaire que pour le développement local
