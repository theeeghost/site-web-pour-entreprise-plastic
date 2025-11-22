BDM Plaste - Plateforme Industrielle Next Gen 🏭✨

📋 À propos du projet

BDM Plaste est une refonte complète de l'expérience digitale pour une industrie de plasturgie. L'objectif est de rompre avec les codes industriels classiques pour proposer une interface immersive, futuriste et haut de gamme.

Le site permet :

La vente directe de produits (E-commerce B2C/B2B).

La gestion de demandes de sous-traitance avec upload de fichiers lourds (3D/CAD).

La prise de rendez-vous interactive.

Une navigation fluide type "Liquid Motion".

🛠 Stack Technique

Ce projet utilise une architecture moderne axée sur la performance et l'animation.

Core

Next.js 14 (App Router) : Framework React pour le SSR et le routing.

TypeScript : Pour un code typé et robuste.

Tailwind CSS : Styling utilitaire (Dark Mode natif).

UI & Animations (Crucial)

Framer Motion : Animations complexes et transitions de pages.

Lenis : Smooth Scroll (défilement inerte premium).

React Three Fiber : (Optionnel) Éléments 3D interactifs.

Backend & Services

CMS : Sanity.io (ou Strapi) - Gestion du contenu catalogue.

Paiement : Stripe - Checkout sécurisé.

Stockage : AWS S3 / Cloudinary - Upload fichiers sous-traitance.

Emails : Resend - Notifications transactionnelles.

🚀 Installation & Démarrage

Prérequis

Node.js v18+

npm ou yarn

1. Cloner le dépôt

git clone [https://github.com/votre-user/bdm-plaste-web.git](https://github.com/votre-user/bdm-plaste-web.git)
cd bdm-plaste-web


2. Installer les dépendances

npm install
# ou
yarn install


3. Configuration des variables d'environnement

Renommez le fichier .env.example en .env.local et remplissez les clés API :

# CMS (Sanity/Strapi)
NEXT_PUBLIC_CMS_PROJECT_ID=votre_id_projet
CMS_API_TOKEN=votre_token_prive

# Paiement (Stripe)
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=pk_test_...
STRIPE_SECRET_KEY=sk_test_...

# Stockage & Emails
NEXT_PUBLIC_AWS_BUCKET_NAME=bdm-uploads
RESEND_API_KEY=re_123...


4. Lancer le serveur de développement

npm run dev


Ouvrez http://localhost:3000 pour voir le résultat.

🎨 Guidelines Design & UI

Le design system repose sur une esthétique Dark Tech / Glassmorphism.

Background : #0B0C15 (Deep Navy). Ne jamais utiliser de blanc pur en fond.

Glass Effect : Utilisez la classe utilitaire glass-panel définie dans globals.css :

.glass-panel {
  @apply bg-white/5 backdrop-blur-xl border border-white/10;
}


Animations :

Toute section doit apparaître avec un FadeUp.

Les boutons doivent avoir un effet magnétique au survol.

📂 Structure du Projet

.
├── components/
│   ├── 3d/            # Modèles et scènes React Three Fiber
│   ├── ui/            # Composants réutilisables (Boutons, Inputs...)
│   ├── layout/        # Header, Footer, SmoothScroll wrapper
│   └── sections/      # Blocs de pages (Hero, Features, Contact)
├── app/               # Next.js 14 App Router
│   ├── page.tsx       # Accueil
│   ├── boutique/      # E-commerce
│   └── sous-traitance/# Formulaire upload
├── lib/               # Fonctions utilitaires, config Stripe/CMS
├── public/            # Assets statiques (fonts, images)
└── styles/            # Globals.css (Tailwind directives)


🤝 Contribution

Créez une branche pour votre fonctionnalité (git checkout -b feature/AmazingFeature).

Commitez vos changements (git commit -m 'Add some AmazingFeature').

Push vers la branche (git push origin feature/AmazingFeature).

Ouvrez une Pull Request.

Projet développé pour BDM Plaste - Tous droits réservés.
