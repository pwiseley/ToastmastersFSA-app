# Toastmasters FSA — Club Management App

Platform built to manage a public speaking club — meetings, members, evaluations, emails, and analytics, all in one place.

🔗 [Live demo](https://toastmastersfsa-app-production.up.railway.app/)

---

<img width="1920" alt="Dashboard" src="https://github.com/user-attachments/assets/64dcfb99-d5ae-4534-b963-86875186e8e8" />
<img width="1920" alt="Meetings" src="https://github.com/user-attachments/assets/ea187f6a-bf6c-4c31-98ab-791c118d74d4" />

---

## Features

**Meeting Management**<br>
└─ `Schedule meetings, assign roles, generate PDF agendas automatically.`

**Member Profiles**<br>
└─ `Track progress, pathways, curriculums, and achievements per member.`

**Speech Evaluations**<br>
└─ `Digital evaluation forms with customizable criteria and feedback.`

**Email Automation**<br>
└─ `Scheduled emails, reminders, and marketing campaigns with a template system.`

**Statistics Dashboard**<br>
└─ `Member activity and club performance metrics — visualized with Chart.js.`

**Role Assignment**<br>
└─ `Automatic role distribution per meeting with conflict detection.`

**Document Management**<br>
└─ `Upload and organize meeting resources, agendas, and materials.`

---

<img width="1920" alt="Email" src="https://github.com/user-attachments/assets/7509deac-74f4-40f7-b3f1-081e8426cbe7" />
<img width="1920" alt="Roles" src="https://github.com/user-attachments/assets/8868ed88-091c-4180-9ee1-a57ebb194e30" />
<img width="1920" alt="Documents" src="https://github.com/user-attachments/assets/7cd95523-95fe-40fb-8329-d743c7c6175c" />
<img width="1275" alt="Overview" src="https://github.com/user-attachments/assets/4c259ac1-35b7-4d0f-9ae6-b09660c03e08" />

---

## User Roles (Authorization)

**Members**
- View schedules, manage their profile, submit speech evaluations.

**Board Members**
- Full access — meeting creation, member management, email campaigns, analytics, club configuration.

*Screenshots above show the board member interface.*

---

## Tech Stack

**Backend**
- Django 5.2, PostgreSQL, Celery, Redis

**Frontend**
- Vanilla JS (AJAX, dynamic forms), Bootstrap 5, Chart.js

**Deployment**
- Docker, Railway (web + PostgreSQL + Redis), Nginx

**Auth & Email**
- Django Allauth, Django SMTP

---

## Project Structure

```
ToastmastersFSA/
├── accounts/          # Authentication, signup, password reset
├── communications/    # Email campaigns, scheduling, templates
├── meetings/          # Meeting management, roles, PDF agendas
├── members/           # Profiles, curriculums, progression
├── speechs/           # Evaluations, criteria, feedback
├── core/              # Shared models and utilities
├── templates/
├── static/
├── media/
├── ToastmastersFSA/   # Django project settings
│   ├── settings.py     
│   ├── urls.py           
│   └── celery.py          
├── docker-compose.yaml  
├── Dockerfile            
├── requirements.txt  
└── manage.py          # Django management script
```

---

## License

MIT — see [LICENSE](LICENSE) for details.

---

[petiton.dev](https://petiton.dev)
