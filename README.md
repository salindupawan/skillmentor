# 🎓 SkillMentor – Online Mentoring Platform

**SkillMentor** is a comprehensive **full-stack mentoring platform** designed to bridge the gap between **students and expert mentors**.

The platform enables specialized learning through **one-on-one mentoring sessions**, **mentor discovery**, and a **streamlined administrative workflow** for managing educational content, bookings, and payments.

---

# 🚀 Live Demo

| Service | Link |
|--------|------|
| Frontend [Repository](https://github.com/salindupawan/skill-mentor-frontend) | https://skilledmentor.vercel.app  |
| Backend API  [Repository](https://github.com/salindupawan/skill-mentor-backend) | https://skillmentor.up.railway.app/swagger-ui/index.html |

---

# 🛠 Tech Stack

| Layer | Technology |
|------|------------|
| **Frontend** | React, TypeScript, Vite, Tailwind CSS, shadcn/ui |
| **Backend** | Spring Boot (Java), Spring Security |
| **Database** | PostgreSQL (Hosted via Supabase) |
| **Authentication** | Clerk (JWT-based Role RBAC) |
| **Deployment** | Vercel (Frontend), Railway (Backend) |

---

# ✨ Key Features

## 🎓 Student Experience

### 🔎 Mentor Discovery
- Advanced search and filtering system for mentors  
- Detailed mentor profile pages with expertise and subjects

### 📅 Session Booking
- Real-time session scheduling  
- Double-booking prevention  
- Past-date validation

### 💳 Payment Workflow
- Upload **bank slip / payment proof**
- Secure payment confirmation workflow

### 📊 Personal Dashboard
Students can:

- Track session status  
- View **Pending / Confirmed / Completed** bookings  
- Access enrolled subjects

---

## 🛡️ Admin Management

### 🔐 Role-Based Access Control

Admin routes are protected:


Only users with **admin role metadata in Clerk** can access these endpoints.

---

### 👨‍🏫 Mentor & Subject Management

Admins can:

- Create mentor profiles
- Approve mentors
- Assign mentors to specific subjects
- Manage subjects through a dedicated UI

---

### 📑 Booking Oversight

Centralized admin dashboard includes:

- Searchable booking table
- Filters for booking status
- Student session tracking

---

### ✅ Validation Logic

Admins can:

- Approve pending payments
- Confirm student bookings
- Mark sessions as completed

---

# 📁 Project Structure

## 📁 Project Structure

```plaintext
skillmentor-platform/
│
├── frontend/                          # React + Vite Frontend Application
│   │
│   ├── public/                        # Static assets
│   │
│   ├── src/
│   │   ├── components/                # Reusable UI components (shadcn/ui, layouts)
│   │   ├── pages/                     # Application pages (Dashboard, Admin, Profile)
│   │   ├── hooks/                     # Custom React hooks (data fetching, auth)
│   │   ├── services/                  # API service layer
│   │   ├── utils/                     # Helper functions and utilities
│   │   ├── types/                     # TypeScript types and interfaces
│   │   ├── App.tsx                    # Root React component
│   │   └── main.tsx                   # Application entry point
│   │
│   ├── index.html
│   └── package.json
│
├── backend/                           # Spring Boot Backend Application
│   │
│   ├── src/main/java/com/skillmentor/
│   │   ├── config/                    # Configuration classes
│   │   ├── controllers/               # REST API controllers
│   │   ├── services/                  # Business logic layer
│   │   ├── repositories/              # JPA repositories
│   │   ├── models/                    # JPA entities (Mentor, Subject, Session)
│   │   ├── dto/                       # Request/Response DTOs
│   │   ├── security/                  # Clerk & Spring Security configuration
│   │   └── SkillMentorApplication.java
│   │
│   └── src/main/resources/
│       └── application.properties
│

│
├── README.md                          # Project documentation
└── .gitignore
```


---




