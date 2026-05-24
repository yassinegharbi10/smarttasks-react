# smarttasks-react
Une application simple de gestion des tâches
Fonctionnalités incluses:
✅ Inscription / Connexion avec validation
✅ Dashboard avec 4 statistiques
✅ CRUD complet (Ajouter, Modifier, Supprimer, Compléter)
✅ Mode sombre (bouton 🌙 dans la navbar)
✅ Recherche de tâches en temps réel
✅ Filtres par statut (Toutes / En attente / Terminées)
✅ Toast notifications (succès, erreur, info)
✅ Responsive mobile/desktop
✅ Routes protégées (redirect si non connecté)
✅ Données persistées en LocalStorage
Arborescence du projet
smarttasks/
├── public/
│   └── index.html
├── src/
│   ├── models/              ← 🔷 Classes POO
│   │   ├── User.js          ← Classe User (id, nom, email, password)
│   │   └── Task.js          ← Classe Task (id, title, description, status, date)
│   ├── context/             ← État global React
│   │   ├── AuthContext.jsx  ← Authentification globale
│   │   └── ThemeContext.jsx ← Mode sombre/clair
│   ├── services/
│   │   └── ToastService.jsx ← Notifications toast
│   ├── routes/
│   │   └── PrivateRoute.jsx ← Protection des routes
│   ├── components/
│   │   ├── Navbar.jsx       ← Barre de navigation
│   │   ├── TaskCard.jsx     ← Carte d'une tâche
│   │   └── StatsCard.jsx    ← Carte statistique
│   ├── pages/
│   │   ├── Login.jsx
│   │   ├── Register.jsx
│   │   ├── Dashboard.jsx
│   │   ├── AddTask.jsx
│   │   └── EditTask.jsx
│   ├── styles/
│   │   └── index.css        ← Design System complet
│   ├── App.jsx              ← Router principal
│   └── index.js
└── package.json
