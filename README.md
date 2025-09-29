# 📦 Carter Cash FAP - Système de Gestion des Expéditions

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/VOTRE_USERNAME/carter-cash-fap)
[![Formspree](https://img.shields.io/badge/Forms-Formspree-blue)](https://formspree.io)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

## 🎯 Description

Interface web professionnelle pour la gestion des commandes et expéditions de Filtres À Particules (FAP) destinée aux magasins Carter Cash.

## ✨ Fonctionnalités

- ✅ **Formulaire de commande intuitif** avec validation
- 📧 **Notifications email automatiques** via Formspree
- 📏 **Saisie des dimensions** et caractéristiques FAP
- 💾 **Sauvegarde automatique** des brouillons
- 📱 **Interface responsive** (mobile/desktop)
- 🔒 **HTTPS sécurisé** avec Vercel
- 📊 **Historique local** des soumissions

## 🚀 Installation Rapide

### Prérequis
- Compte [GitHub](https://github.com)
- Compte [Formspree](https://formspree.io) (gratuit)
- Compte [Vercel](https://vercel.com) (gratuit)

### Étapes

1. **Fork ce repository**
   ```bash
   # Ou cloner localement
   git clone https://github.com/VOTRE_USERNAME/carter-cash-fap.git
   cd carter-cash-fap
   ```

2. **Configurer Formspree**
   - Créer un formulaire sur [formspree.io](https://formspree.io)
   - Copier l'endpoint (format: `https://formspree.io/f/XXXXX`)

3. **Modifier l'endpoint**
   - Ouvrir `index.html`
   - Remplacer `VOTRE_ID` par votre endpoint Formspree (ligne 386)

4. **Déployer sur Vercel**
   - Connecter GitHub à Vercel
   - Importer ce repository
   - Deploy automatique !

## 📝 Configuration

### Endpoint Formspree

Dans `index.html`, ligne 386 :
```html
<form id="expeditionForm" action="https://formspree.io/f/VOTRE_ID" method="POST">
```

### Ajouter un magasin

Dans `index.html`, ajouter une option :
```html
<option value="Carter Cash Ville">Carter Cash Ville</option>
```

### Personnalisation des couleurs

Modifier le gradient dans le CSS :
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

## 📁 Structure du Projet

```
carter-cash-fap/
├── index.html          # Interface principale
├── README.md           # Documentation
├── LICENSE            # Licence MIT
├── .gitignore         # Fichiers ignorés
└── vercel.json        # Configuration Vercel
```

## 🔧 Développement Local

```bash
# Cloner le repository
git clone https://github.com/VOTRE_USERNAME/carter-cash-fap.git
cd carter-cash-fap

# Ouvrir dans le navigateur
open index.html

# Ou utiliser un serveur local
python -m http.server 8000
# Puis ouvrir http://localhost:8000
```

## 📊 Gestion des Données

### Réception des soumissions
- **Email** : Directement dans votre boîte
- **Formspree Dashboard** : [formspree.io/forms](https://formspree.io/forms)
- **Export CSV** : Disponible dans Formspree
- **Google Sheets** : Intégration possible via Formspree

### Stockage local
- Brouillons sauvegardés automatiquement
- Historique des 50 dernières soumissions
- Données dans `localStorage`

## 🚀 Déploiement

### Option 1 : Vercel (Recommandé)
1. Push sur GitHub
2. Connecter à Vercel
3. Deploy automatique à chaque commit !

### Option 2 : Netlify
1. Drag & drop du dossier
2. URL instantanée

### Option 3 : GitHub Pages
1. Settings → Pages
2. Source : main branch
3. Disponible sur `username.github.io/carter-cash-fap`

## 🔒 Sécurité

- ✅ HTTPS automatique avec Vercel
- ✅ Protection anti-spam Formspree
- ✅ Validation côté client
- ✅ Pas de données sensibles stockées

## 📈 Statistiques

Vercel Analytics disponible gratuitement :
- Nombre de visiteurs
- Temps de chargement
- Taux de soumission

## 🛠️ Maintenance

### Mise à jour de l'interface
```bash
git add .
git commit -m "Description des changements"
git push origin main
# Vercel redéploie automatiquement !
```

### Vérifier les logs
- Formspree : Dashboard → Submissions
- Vercel : Dashboard → Functions logs

## 📱 Support Navigateurs

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Mobile iOS/Android

## 🤝 Contribution

Les contributions sont bienvenues ! 
1. Fork le projet
2. Créer une branche (`git checkout -b feature/amelioration`)
3. Commit (`git commit -m 'Ajout de...'`)
4. Push (`git push origin feature/amelioration`)
5. Ouvrir une Pull Request

## 📄 Licence

Ce projet est sous licence MIT - voir [LICENSE](LICENSE) pour plus de détails.

## 📞 Support

- **Documentation** : Ce README
- **Issues** : [GitHub Issues](https://github.com/VOTRE_USERNAME/carter-cash-fap/issues)
- **Email** : support@votre-entreprise.com

## 🎉 Remerciements

- [Formspree](https://formspree.io) pour le traitement des formulaires
- [Vercel](https://vercel.com) pour l'hébergement
- Équipe Carter Cash pour la collaboration

---

**Version** : 1.0.0  
**Dernière mise à jour** : Décembre 2024  
**Statut** : ✅ Production Ready