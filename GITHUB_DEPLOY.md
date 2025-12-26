# 📦 Guide de déploiement sur GitHub Pages

## Étape 1 : Créer un compte GitHub (si vous n'en avez pas)

1. Allez sur https://github.com
2. Cliquez sur "Sign up"
3. Créez votre compte (gratuit)

## Étape 2 : Créer un nouveau dépôt (repository)

1. Connectez-vous à GitHub
2. Cliquez sur le bouton "+" en haut à droite
3. Sélectionnez "New repository"
4. Nommez-le : `checkrisk` (ou un autre nom)
5. Cochez "Public" (gratuit pour GitHub Pages)
6. **NE COCHEZ PAS** "Initialize this repository with a README"
7. Cliquez sur "Create repository"

## Étape 3 : Préparer et envoyer vos fichiers

Exécutez ces commandes dans le terminal (dans le dossier CheckRisk) :

```bash
# Vérifier que vous êtes dans le bon dossier
cd /Users/zlatashvets/CheckRisk

# Ajouter tous les fichiers (sauf node_modules)
git add index.html README.md DEPLOY.md netlify.toml .gitignore package.json

# Créer le premier commit
git commit -m "Initial commit - CheckRisk website"

# Renommer la branche en main (si nécessaire)
git branch -M main

# Ajouter le dépôt distant (remplacez VOTRE-USERNAME par votre nom d'utilisateur GitHub)
git remote add origin https://github.com/VOTRE-USERNAME/checkrisk.git

# Envoyer les fichiers sur GitHub
git push -u origin main
```

**Important :** Remplacez `VOTRE-USERNAME` par votre vrai nom d'utilisateur GitHub dans la commande `git remote add origin`.

## Étape 4 : Activer GitHub Pages

1. Allez sur votre dépôt GitHub (https://github.com/VOTRE-USERNAME/checkrisk)
2. Cliquez sur "Settings" (en haut du dépôt)
3. Dans le menu de gauche, cliquez sur "Pages"
4. Sous "Source", sélectionnez :
   - Branch: `main`
   - Folder: `/ (root)`
5. Cliquez sur "Save"
6. Attendez 1-2 minutes

## Étape 5 : Accéder à votre site

Votre site sera disponible sur :
**https://VOTRE-USERNAME.github.io/checkrisk**

(Remplacez VOTRE-USERNAME par votre nom d'utilisateur GitHub)

## 🔄 Mettre à jour le site

Quand vous modifiez des fichiers, exécutez :

```bash
git add .
git commit -m "Description des changements"
git push
```

Les changements seront en ligne dans 1-2 minutes.

## ❓ Problèmes courants

**Erreur "remote origin already exists" :**
```bash
git remote remove origin
git remote add origin https://github.com/VOTRE-USERNAME/checkrisk.git
```

**Demande de nom d'utilisateur/mot de passe :**
- Utilisez un Personal Access Token au lieu du mot de passe
- Créez-en un dans GitHub Settings > Developer settings > Personal access tokens

