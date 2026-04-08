> 🇬🇧 [Read in English](README.md)

# Toastmasters FSA — Application de gestion de club

Plateforme conçue pour gérer un club d'art oratoire — réunions, membres, évaluations, courriels et analytiques, le tout en un seul endroit.

🔗 [Démo en ligne](https://toastmastersfsa-app-production.up.railway.app/)

---

## 📸 Captures d'écran

*Authentification*
<img width="1920" alt="authentication" src="https://github.com/user-attachments/assets/64dcfb99-d5ae-4534-b963-86875186e8e8" />

*Tableau de bord*
<img width="1920" alt="Meetings" src="https://github.com/user-attachments/assets/ea187f6a-bf6c-4c31-98ab-791c118d74d4" />

*Planification des réunions et assignation des rôles*
<img width="1920" alt="Email" src="https://github.com/user-attachments/assets/7509deac-74f4-40f7-b3f1-081e8426cbe7" />

*Gestion du club*
<img width="1920" alt="Roles" src="https://github.com/user-attachments/assets/8868ed88-091c-4180-9ee1-a57ebb194e30" />

*Campagnes courriel et planification*
<img width="1920" alt="Documents" src="https://github.com/user-attachments/assets/7cd95523-95fe-40fb-8329-d743c7c6175c" />

*Envoi de courriels planifiés en action*
<img width="1275" alt="Overview" src="https://github.com/user-attachments/assets/4c259ac1-35b7-4d0f-9ae6-b09660c03e08" />

---

## Fonctionnalités

**Gestion des réunions**<br>
└─ `Planification des réunions, assignation des rôles, génération automatique d'ordres du jour en PDF.`

**Profils des membres**<br>
└─ `Suivi de la progression, des parcours, des curriculums et des accomplissements par membre.`

**Évaluations de discours**<br>
└─ `Formulaires d'évaluation numériques avec critères personnalisables et rétroaction.`

**Automatisation des courriels**<br>
└─ `Courriels planifiés, rappels et campagnes marketing avec système de gabarits.`

**Tableau de bord analytique**<br>
└─ `Activité des membres et métriques de performance du club, visualisées avec Chart.js.`

**Assignation des rôles**<br>
└─ `Distribution automatique des rôles par réunion avec détection des conflits.`

**Gestion des documents**<br>
└─ `Téléversement et organisation des ressources de réunion, ordres du jour et documents.`

---

## Rôles utilisateurs (autorisation)

**Membres**
- Consulter les horaires, gérer leur profil, soumettre des évaluations de discours.

**Membres du conseil**
- Accès complet : création de réunions, gestion des membres, campagnes courriel, analytiques, configuration du club.

*Les captures d'écran ci-dessus montrent l'interface des membres du conseil.*

---

## Technologies

**Backend**
- Django 5.2, PostgreSQL, Celery, Redis

**Frontend**
- Vanilla JS (AJAX, formulaires dynamiques), Bootstrap 5, Chart.js

**Déploiement**
- Docker, Railway (web + PostgreSQL + Redis), Nginx

**Authentification et courriel**
- Django Allauth, Django SMTP

---

## Structure du projet

```
ToastmastersFSA/
├── accounts/          # Authentification, inscription, réinitialisation du mot de passe
├── communications/    # Campagnes courriel, planification, gabarits
├── meetings/          # Gestion des réunions, rôles, ordres du jour PDF
├── members/           # Profils, curriculums, progression
├── speechs/           # Évaluations, critères, rétroaction
├── core/              # Modèles et utilitaires partagés
├── templates/
├── static/
├── media/
├── ToastmastersFSA/   # Paramètres du projet Django
│   ├── settings.py
│   ├── urls.py
│   └── celery.py
├── docker-compose.yaml
├── Dockerfile
├── requirements.txt
└── manage.py          # Script de gestion Django
```

---

## Licence

MIT — voir [LICENSE](LICENSE) pour les détails.

---

[petiton.dev](https://petiton.dev)
