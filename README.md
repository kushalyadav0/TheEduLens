# 🎓 TheEduLens

> Shining a lens on student learning progress.

TheEduLens is a modular, API-driven student progress tracking and automation platform designed to support educational programs, facilitators, and learners. Built with Django REST Framework (backend) and a modern frontend stack, it provides powerful insights into student attendance, assignment completion, course milestones, and engagement trends.

---

## 🚀 Key Features

- 📊 **Dashboard View**: See student metrics in real time (attendance, scores, engagement).
- 📝 **Assignment Tracker**: Monitor submission status, feedback, and grading.
- 📅 **Attendance System**: Easy logging with visual summaries.
- 📈 **Progress Charts**: Visualize growth using Plotly or Chart.js.
- 🔁 **Automated Alerts**: Notify facilitators or students of low attendance, pending tasks, etc.
- 🔗 **External Integrations**: Easily connect with Google Sheets, Slack, email, or other services via APIs or n8n.
- 🔐 **JWT Authentication**: Secure, scalable login and token management.

---

## 🧱 Tech Stack

### 🔧 Backend
- Python 3.12
- Django + Django REST Framework
- PostgreSQL
- Pandas (for reporting/automation)
- SimpleJWT (for authentication)
- Celery + Redis (planned for background tasks)

### 🎨 Frontend
- HTML + Tailwind CSS (WIP) + JS
- Chart.js / Plotly (for analytics)

### 🔁 Automation / Integration
- n8n (self-hosted workflows)
- Django EmailBackend
- Scheduled scripts (Python + CRON/Celery)

---

## 📁 Project Structure

```
theedulens/
├── backend/              # Django + DRF API
│   ├── core/             # Models, views, serializers
│   └── api/              # Versioned API endpoints
├── frontend/             # React or JS-based dashboard UI
│   └── public/           # Static files and assets
├── docs/                 # Architecture, API docs, wireframes
└── README.md             # This file
```

---

## 🛠️ Setup Instructions

### Backend (Django)
```bash
cd backend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

### Frontend (React / HTML)
```bash
cd frontend
npm install
npm start
```

---

## 🌐 API Overview

| Method | Endpoint              | Purpose               |
|--------|------------------------|------------------------|
| POST   | `/api/token/`         | Get JWT tokens         |
| GET    | `/api/students/`      | List students          |
| POST   | `/api/attendance/`    | Mark attendance        |
| GET    | `/api/progress/<id>/` | Get student progress   |

Full API docs available [here](docs/API_REFERENCE.md) _(coming soon)_

---

## 🧠 Vision

> To create transparent, data-informed educational tools that support human learning, discipline, and dignity.

This project was inspired by a social impact internship opportunity at **Work With Dignity Foundation** and is intended to evolve into a reusable backend-agnostic framework for educational tracking, automation, and insights.

---

## 📌 Roadmap

- [x] Backend API scaffolding
- [x] Attendance & assignment models
- [ ] JWT-based login/signup
- [ ] Frontend dashboard
- [ ] Plotly visualizations
- [ ] n8n automation workflows
- [ ] Admin alerts via email/Slack
- [ ] Deployment (Docker + Render/Fly.io)

---

## 🙋‍♂️ Author

**Kushal Yadav**  
Electrical & Electronics Engineering Student  
[GitHub: @kushalyadav0](https://github.com/kushalyadav0)  
[LinkedIn](https://linkedin.com/in/kushal-yadav-799310318)

---

## 📄 License

MIT License (Open to collaboration and contributions)
