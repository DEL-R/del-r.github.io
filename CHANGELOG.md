# Changelog

## [2.0.0] - 2025-01-30

### 🚀 Modernisation majeure de la stack technique

#### Ajouté
- **Jekyll 4.3.4** - Migration de la version 3.x vers 4.x
- **Ruby 3.3.7** - Mise à jour depuis Ruby 2.x
- **Plugins Jekyll modernes** :
  - `jekyll-sitemap` pour le SEO
  - `jekyll-feed` pour les flux RSS
  - `jekyll-seo-tag` pour l'optimisation SEO
- **Support Markdown moderne** :
  - `kramdown` 2.5.1 avec `kramdown-parser-gfm`
  - Support GitHub Flavored Markdown complet
- **Coloration syntaxique** : `rouge` 4.6.0
- **Configuration moderne** :
  - `.ruby-version` pour la gestion des versions
  - `package.json` avec scripts npm/yarn
  - `.gitignore` mis à jour pour les outils modernes

#### Modifié
- **Gemfile** complètement réécrit avec les meilleures pratiques
- **Configuration Jekyll** (`_config.yml`) modernisée pour Jekyll 4.x
- **README.md** complet avec instructions modernes
- **Structure des dépendances** :
  - Installation locale des gems dans `vendor/bundle`
  - Gems futures Ruby 3.4+ (`csv`, `base64`)
  - Support Faraday moderne avec `faraday-retry`

#### Supprimé
- **Bower** remplacé par npm/yarn
- **Ancien Gemfile.lock** pour forcer la régénération
- **bower_components/** obsolète
- **Dépendances obsolètes** et vulnérables

#### Sécurité
- ✅ **Toutes les vulnérabilités** des anciennes dépendances corrigées
- ✅ **Dépendances à jour** avec les dernières versions stables
- ✅ **Ruby moderne** avec correctifs de sécurité

### 🛠 Améliorations techniques

#### Performance
- **Cache Jekyll** activé pour des builds plus rapides
- **Installation locale** des gems pour éviter les conflits
- **Build optimisé** avec Jekyll 4.x

#### SEO et accessibilité
- **Jekyll SEO Tag** pour métadonnées optimisées
- **Sitemap automatique** pour l'indexation
- **Flux RSS** moderne avec Jekyll Feed

---

## [1.0.0] - 2016-12-11

### Version initiale
- Site Jekyll 3.x avec theme custom
- Support Bower pour les dépendances front-end
- Article "Jekyll et Foundation"
- Configuration de base avec Disqus et Google Analytics