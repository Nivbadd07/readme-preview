# 🌐 RooMatch – Cloud-Native Roommate Matching Platform

**RooMatch** is a next-generation, cloud-native platform designed to intelligently match roommates based on lifestyle compatibility, behavioral traits, and housing preferences. Built as part of my B.Sc. in Information Systems capstone, RooMatch showcases real-world, production-grade engineering using modern DevOps, microservices, and AI-aligned principles.

---

## ✨ Key Features

* 🖥️ Fully responsive single-page frontend using HTML, CSS, JavaScript, and TailwindCSS.
* 🧠 AI-enhanced Python (Flask) match engine that calculates compatibility scores.
* ☁️ Direct, secure file uploads from browser to Google Cloud Storage via signed URLs.
* 🔁 Stateless microservices deployed on Google Cloud Run with auto-scaling and zero-downtime revisioning.
* 🗄️ Supabase PostgreSQL for relational data and JWT-based access control.
* 🚀 CI/CD pipeline with GitHub Actions, Cloud Build, and Artifact Registry for fast, automated delivery.

---

## 🛠️ Tech Stack Overview

| Layer          | Technologies                                                              |
| -------------- | ------------------------------------------------------------------------- |
| Frontend       | HTML, CSS, JavaScript, TailwindCSS, Vite                                  |
| Match Engine   | Python 3.12 (Flask), modular microservice architecture                    |
| Data Layer     | Supabase PostgreSQL, JWT auth, pgvector (planned)                         |
| File Storage   | Google Cloud Storage, signed URL uploads                                  |
| Cloud Services | Google Cloud Run, Load Balancing, Artifact Registry, Secret Manager       |
| DevOps & IaC   | GitHub Actions, Cloud Build, Terraform, Build Triggers, Rollback Handling |

---

## 🧭 System Architecture

```
                   ┌────────────────────┐
                   │     Frontend       │
                   │  (HTML/CSS/JS)     │
                   └────────┬───────────┘
                            │
                            ▼
        ┌────────────────────────────────────┐
        │ Google Cloud Storage (Static Site)│
        └────────────────┬───────────────────┘
                         │
                         ▼
        ┌────────────────────────────────────┐
        │ Python Match Engine (Flask, REST) │
        └────────────────┬───────────────────┘
                         │
                         ▼
        ┌────────────────────────────────────┐
        │ Supabase (PostgreSQL + JWT Auth)  │
        └────────────────────────────────────┘
                         ▲
                         │
        ┌────────────────────────────────────┐
        │ CI/CD: GitHub Actions → Cloud Build│
        │        → Artifact Registry → Deploy│
        └────────────────────────────────────┘
```

---

## 🚢 Deployment

* 🌍 **Frontend**: [RooMatch Static Site](http://storage.googleapis.com/roomatch-prod-static-site/index.html)
* ⚙️ **Match Engine & Services**: Hosted on Google Cloud Run with traffic control, logs, secrets, and automatic revisioning.

---

## 🔮 Planned Enhancements

* 🔐 Google OAuth 2.0 for SSO.
* 🧬 AI-based matching using OpenAI embeddings + pgvector.
* 🔔 Firebase Cloud Messaging for push notifications.
* 📱 React Native mobile application.
* ✅ End-to-end test suite (unit, integration, Cypress).

---

## 👨‍💻 Author

**Niv Badash**
Cloud-native full-stack developer with a passion for intelligent architecture and automated delivery pipelines.
📩 [nivbadd@gmail.com](mailto:nivbadd@gmail.com)

---

## 🤝 Collaboration

Whether it's feedback, code contributions, or technical partnerships—I'm open to ideas. Reach out directly or submit a GitHub issue to collaborate.

---

> 🚀 RooMatch blends smart logic and modern infrastructure to transform how roommates discover each other in the digital age.
