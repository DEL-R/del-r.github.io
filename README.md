# Le Lab' RD

Site personnel de Rudy Delansay - Développeur passionné par l'Open-Source

## 🚀 Technologies

- **Jekyll 4.3.x** - Générateur de site statique
- **Ruby 3.3+** - Langage de programmation
- **Bootstrap 5** - Framework CSS moderne
- **Rouge** - Coloration syntaxique
- **Kramdown** - Processeur Markdown

## 📋 Prérequis

- **Ruby** >= 3.3.0
- **Bundler** >= 2.0
- **Node.js** >= 16.0 (optionnel, pour les dépendances front-end)

## 🛠 Installation

### 1. Cloner le repository
```bash
git clone https://github.com/del-r/del-r.github.io.git
cd del-r.github.io
```

### 2. Installer les dépendances Ruby
```bash
bundle config set --local path 'vendor/bundle'
bundle install
```

### 3. (Optionnel) Installer les dépendances Node.js
```bash
npm install
```

## 🎯 Utilisation

### Développement local
```bash
# Serveur de développement standard
bundle exec jekyll serve

# Avec live-reload et brouillons
bundle exec jekyll serve --livereload --drafts
```

Le site sera accessible sur `http://localhost:4000`

### Construction du site
```bash
bundle exec jekyll build
```

### Nettoyage
```bash
bundle exec jekyll clean
```

## 📁 Structure

```
├── _config.yml          # Configuration Jekyll
├── _posts/              # Articles de blog
├── _includes/           # Composants réutilisables
├── _layouts/            # Templates de page
├── _sass/               # Fichiers SCSS
├── assets/              # Ressources statiques
├── Gemfile              # Dépendances Ruby
└── README.md            # Ce fichier
```

## 🔧 Configuration

### Jekyll
La configuration principale se trouve dans `_config.yml`. Les paramètres importants :

- `title` : Titre du site
- `description` : Description pour le SEO
- `url` : URL de production
- `plugins` : Plugins Jekyll activés

### Analytics
Configurez Google Analytics dans `_config.yml` :
```yaml
analytics:
  google:
    tracking_id: 'VOTRE_ID_TRACKING'
```

## 📝 Créer du contenu

### Nouvel article
```bash
# Créer un fichier dans _posts/
# Format : YYYY-MM-DD-titre-de-l-article.md

# Exemple :
_posts/2024-01-15-mon-nouvel-article.md
```

### Front Matter obligatoire
```yaml
---
layout: post
title: "Titre de l'article"
date: 2024-01-15 10:00:00 +0100
categories: [webdev, tutorial]
tags: [jekyll, markdown]
---
```

## 🚀 Déploiement

### GitHub Pages (automatique)
Le site se déploie automatiquement sur `https://del-r.github.io` lors des push sur `main`.

### Autre hébergement
1. Construire le site : `bundle exec jekyll build`
2. Déployer le contenu du dossier `_site/`

## 🐛 Dépannage

### Problèmes courants

**Erreur Bundler :**
```bash
bundle update
```

**Erreur de gems manquantes :**
```bash
bundle install --redownload
```

**Problème de version Ruby :**
Vérifiez que Ruby >= 3.3.0 est installé :
```bash
ruby --version
```

## 📄 Licence

Ce projet est sous licence Apache 2.0. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 🤝 Contribution

Les contributions sont les bienvenues ! N'hésitez pas à :
- Signaler des bugs
- Proposer des améliorations
- Soumettre des pull requests

## 📧 Contact

- **Email** : delansay.rudy@gmail.com
- **GitHub** : [@del-r](https://github.com/del-r)
- **Site** : [https://del-r.github.io](https://del-r.github.io)