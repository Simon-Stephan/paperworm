# PaperWorm

**PaperWorm** est une plateforme de gestion de projets de recherche académique, conçue pour aider les chercheurs à organiser leurs travaux, collaborer efficacement et optimiser le processus de recherche scientifique.

## 📖 À propos

PaperWorm permet aux chercheurs et équipes académiques de gérer l'ensemble du cycle de vie d'un projet de recherche scientifique, de la formulation des questions de recherche à l'analyse des publications, en passant par le suivi des tâches et la collaboration entre membres d'équipe.

L'application est développée en Next.js (React) avec TypeScript, offrant une interface utilisateur moderne et réactive, et une architecture robuste pour gérer efficacement les projets de recherche complexes.

## ✨ Fonctionnalités

### Organisation de la recherche
- **Questions scientifiques**: Définissez la question scientifique principale de votre projet.
- **Questions de recherche**: Décomposez votre recherche en questions spécifiques à traiter.
- **Questions d'étude**: Créez des questionnaires pour analyser systématiquement les publications.

### Gestion de la littérature
- **Publications**: Importez, organisez et analysez les publications scientifiques.
- **Requêtes de recherche**: Construisez des requêtes pour explorer la littérature scientifique.
- **Mots-clés**: Gérez un vocabulaire contrôlé pour catégoriser vos publications.

### Collaboration et suivi
- **Forum de discussion**: Communiquez avec les membres de votre équipe sur des sujets spécifiques.
- **Kanban**: Suivez l'avancement des tâches avec un tableau Kanban.
- **Processus**: Modélisez et documentez vos processus de recherche.

### Rapports et analyses
- **Rapports**: Générez des rapports sur l'avancement de votre recherche.
- **Statistiques**: Visualisez des statistiques sur l'état de votre projet.

## 🛠️ Technologies utilisées

- **Frontend**: Next.js (React), TypeScript, Tailwind CSS
- **Authentification**: JWT
- **UI Components**: Composants personnalisés avec Tailwind
- **Gestion d'état**: React Context API
- **Internationalisation**: Support multilingue (Français/Anglais)

## 📦 Structure du projet

```
src/
├── app/                  # Routes et pages de l'application (Next.js App Router)
├── components/           # Composants réutilisables
│   ├── auth/             # Composants d'authentification
│   ├── dashboard/        # Composants du tableau de bord
│   ├── project/          # Composants spécifiques aux projets
│   └── ui/               # Composants d'interface utilisateur de base
├── contexts/             # Contextes React
├── lib/                  # Bibliothèques et utilitaires
│   ├── api/              # Services d'API
│   ├── types/            # Types TypeScript
│   └── utils/            # Fonctions utilitaires
└── styles/               # Styles globaux
```

## 🗃️ Modèles de données

Le système est organisé autour de plusieurs entités principales:

- **Project**: Contient les métadonnées du projet et regroupe toutes les autres entités.
- **ScientificQuestion**: La question scientifique principale du projet.
- **ResearchQuestion**: Les questions de recherche spécifiques.
- **StudyQuestion**: Les questions d'étude pour analyser les publications.
- **Publication**: Les publications scientifiques importées.
- **Keyword**: Les mots-clés pour catégoriser les publications.
- **Query**: Les requêtes de recherche pour explorer la littérature.
- **ForumTopic/ForumReply**: Les discussions au sein du projet.
- **KanbanTask**: Les tâches à réaliser dans le projet.
- **Process**: Les processus de recherche modélisés.

## 🚀 Installation et démarrage

### Prérequis
- Node.js (v16+)
- npm ou yarn

### Installation

```bash
# Cloner le dépôt
git clone https://github.com/simon-stephan/paperworm.git
cd paperworm

# Installer les dépendances
npm install
# ou
yarn install

# Configurer les variables d'environnement
cp .env.example .env.local
# Puis modifiez .env.local avec vos propres valeurs

# Lancer le serveur de développement
npm run dev
# ou
yarn dev
```

L'application sera accessible à l'adresse [http://localhost:3000](http://localhost:3000).

## 🔒 Authentification

L'application utilise JWT pour l'authentification. Les utilisateurs peuvent:
- S'inscrire avec un email et un mot de passe
- Se connecter à leur compte
- Réinitialiser leur mot de passe

## 📋 Guide d'utilisation

### Créer un nouveau projet
1. Connectez-vous à votre compte
2. Dans le tableau de bord, cliquez sur "Nouveau projet"
3. Remplissez les informations de base du projet
4. Commencez à ajouter des membres, des questions de recherche, etc.

### Gérer les publications
1. Dans un projet, accédez à la section "Publications"
2. Importez des publications manuellement ou via des requêtes
3. Analysez les publications en répondant aux questions d'étude

### Collaborer avec d'autres chercheurs
1. Invitez des membres à rejoindre votre projet via la section "Paramètres > Membres"
2. Assignez des rôles (propriétaire, éditeur, lecteur)
3. Communiquez via le forum du projet

## 👥 Contribuer

Les contributions sont les bienvenues! Si vous souhaitez contribuer à ce projet:

1. Forkez le dépôt
2. Créez une branche pour votre fonctionnalité (`git checkout -b feature/amazing-feature`)
3. Committez vos changements (`git commit -m 'Add some amazing feature'`)
4. Poussez vers la branche (`git push origin feature/amazing-feature`)
5. Ouvrez une Pull Request

Veuillez consulter le fichier CONTRIBUTING.md pour les détails sur notre code de conduite et le processus de soumission des pull requests.

## 📝 Feuille de route

- [ ] Intégration avec des API de bases de données académiques (Scopus, Web of Science, etc.)
- [ ] Extraction automatique de métadonnées à partir de PDF
- [ ] Outils d'annotation de PDF
- [ ] Analyse statistique avancée des données bibliométriques
- [ ] Export de bibliographie au format BibTeX, RIS, etc.
- [ ] Intégration avec des outils de gestion de références (Zotero, Mendeley)

## 📜 Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE.md](LICENSE.md) pour plus de détails.

## 📞 Contact

Pour toute question ou suggestion, n'hésitez pas à nous contacter:

- Email: hello@simonstephan.fr
- Site web: [https://paperworm.org](https://paperworm.org)

---

Développé avec ❤️ par l'équipe PaperWorm pour faciliter la recherche académique.
