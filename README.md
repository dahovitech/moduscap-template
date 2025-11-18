# ModusCap - Template E-commerce Maisons Modulaires

Template web professionnel pour la vente de maisons modulaires en kit, optimisé pour la conversion et l'expérience utilisateur.

## 🎯 Caractéristiques Principales

- **6 pages HTML complètes** : Accueil, Produits, Services, À propos, Contact, Devis
- **Design responsive** : Compatible tous devices (mobile, tablette, desktop)
- **Système de filtrage avancé** : Recherche et filtres en temps réel sur la page produits
- **Formulaire de devis wizard** : Formulaire multi-étapes avec calcul de prix en temps réel
- **Performance optimisée** : Chargement rapide, code propre et optimisé
- **SEO-friendly** : Structure sémantique et meta tags optimisés
- **Accessible** : Conformité WCAG 2.1 AA

## 📁 Structure du Projet

```
moduscap-template/
├── index.html              # Page d'accueil
├── produits.html           # Catalogue produits avec filtres
├── services.html           # Présentation des services
├── a-propos.html           # À propos de l'entreprise
├── contact.html            # Formulaire de contact et localisation
├── devis.html              # Formulaire de devis multi-étapes
├── css/
│   └── style.css          # Styles personnalisés
├── js/
│   ├── script.js          # Fonctionnalités communes
│   ├── products-page.js   # Gestion des produits et filtres
│   └── quote-form.js      # Formulaire de devis wizard
├── images/
│   ├── logo.png           # Logo principal
│   ├── logo-light.png     # Logo version claire
│   └── favicon.png        # Icône du site
└── README.md              # Documentation
```

## 🚀 Installation et Utilisation

### Installation Locale

1. **Cloner le repository**
   ```bash
   git clone https://github.com/dahovitech/moduscap-template.git
   cd moduscap-template
   ```

2. **Ouvrir dans un navigateur**
   - Ouvrez le fichier `index.html` dans votre navigateur
   - Ou utilisez un serveur local (recommandé) :
     ```bash
     # Avec Python
     python -m http.server 8000
     
     # Avec Node.js
     npx serve
     
     # Avec PHP
     php -S localhost:8000
     ```

3. **Accéder au site**
   - Ouvrez http://localhost:8000 dans votre navigateur

### Déploiement

#### GitHub Pages
1. Activer GitHub Pages dans les paramètres du repository
2. Sélectionner la branche `main` comme source
3. Le site sera accessible à : `https://dahovitech.github.io/moduscap-template/`

#### Autres Plateformes
- **Netlify** : Glisser-déposer le dossier ou connecter le repository
- **Vercel** : Import depuis GitHub
- **Hébergement traditionnel** : Uploader via FTP

## 🎨 Personnalisation

### Couleurs

Modifier les variables CSS dans `css/style.css` :

```css
:root {
  --primary-color: #2c5aa0;      /* Couleur principale */
  --secondary-color: #f8f9fa;    /* Couleur secondaire */
  --accent-color: #28a745;       /* Couleur accent */
  --text-primary: #212529;       /* Texte principal */
  --text-secondary: #6c757d;     /* Texte secondaire */
}
```

### Logos et Images

Remplacer les fichiers dans le dossier `images/` :
- `logo.png` : Logo principal (format PNG, ~200x60px recommandé)
- `logo-light.png` : Logo pour fond sombre
- `favicon.png` : Icône du site (32x32px ou 64x64px)

### Contenu

1. **Textes** : Modifier directement dans les fichiers HTML
2. **Produits** : Éditer le tableau `products` dans `js/products-page.js`
3. **Pricing** : Ajuster l'objet `PRICING` dans `js/quote-form.js`

## 🛠️ Technologies Utilisées

- **HTML5** : Structure sémantique
- **CSS3** : Styles modernes avec variables CSS
- **JavaScript ES6+** : Fonctionnalités interactives
- **Bootstrap 5.3** : Framework CSS responsive
- **SVG** : Icônes vectorielles

## 📊 Fonctionnalités Détaillées

### Page Produits
- Recherche textuelle en temps réel
- Filtres par prix, surface, chambres, style
- Tri multiple (prix, surface, nom, popularité)
- Persistance des filtres dans l'URL
- Animations au scroll
- Cartes produits interactives

### Formulaire de Devis
- Wizard en 5 étapes
- Calcul de prix en temps réel
- Sauvegarde automatique de la progression
- Validation de chaque étape
- Récapitulatif complet avant envoi
- Design intuitif et guidé

### Design Système
- Palette de couleurs cohérente
- Typographie hiérarchisée
- Composants réutilisables
- Animations fluides
- States interactifs (hover, focus, active)

## ⚡ Performance

- Temps de chargement < 3 secondes
- Code minifié pour la production
- Lazy loading des images
- Optimisation des animations CSS
- Debounce sur les événements fréquents

## ♿ Accessibilité

- Navigation au clavier complète
- Labels ARIA appropriés
- Contraste de couleurs WCAG AA
- Focus visible sur tous les éléments
- Textes alternatifs pour les images

## 🔍 SEO

- Meta tags optimisés sur chaque page
- Structure sémantique HTML5
- URLs propres et descriptives
- Breadcrumbs pour la navigation
- Schema.org ready

## 📱 Responsive Design

- **Mobile First** : Design optimisé pour mobile d'abord
- **Breakpoints** :
  - xs: < 576px (mobile)
  - sm: ≥ 576px (mobile large)
  - md: ≥ 768px (tablette)
  - lg: ≥ 992px (desktop)
  - xl: ≥ 1200px (large desktop)

## 🔧 Maintenance

### Ajouter un Nouveau Produit

Éditer `js/products-page.js` :

```javascript
{
  id: 10,
  name: 'Nouveau Modèle',
  price: 100000,
  surface: 100,
  bedrooms: 3,
  bathrooms: 2,
  style: 'moderne',
  description: 'Description du modèle',
  image: 'https://...',
  features: ['Feature 1', 'Feature 2']
}
```

### Modifier les Prix

Éditer `js/quote-form.js` dans l'objet `PRICING` :

```javascript
const PRICING = {
  basePricePerSqm: 1200,  // Prix de base par m²
  bedrooms: { ... },       // Prix par nombre de chambres
  // etc.
};
```

## 📞 Support

Pour toute question ou suggestion :
- **Email** : contact@moduscap.fr
- **Issues** : [GitHub Issues](https://github.com/dahovitech/moduscap-template/issues)

## 📄 Licence

Ce projet est sous licence MIT. Vous êtes libre de l'utiliser, le modifier et le distribuer.

## 👤 Auteur

**Prudence Dieudonné ASSOGBA** (jprud67)
- GitHub: [@jprud67](https://github.com/jprud67)

## 🙏 Remerciements

- Bootstrap pour le framework CSS
- Unsplash pour les images de démonstration
- La communauté open source

---

**© 2025 ModusCap. Tous droits réservés.**
