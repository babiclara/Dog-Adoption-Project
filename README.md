# Dog Adoption Project

This project is a full-stack **Dog Adoption Platform** built as part of my thesis at **Algebra Bernays University**.  
It consists of three main components: a **mobile app**, a **web admin dashboard**, and a **backend API**.  
Together, they provide a complete system for browsing, managing, and facilitating dog adoptions.  

---

## 📱 Mobile App
- **Repository:** [dog-adoption-app](https://github.com/babiclara/dog-adoption-app)  
- **Tech stack:** Kotlin, Jetpack Compose, Android Studio  
- **Features:**
  - User registration & login (JWT authentication)  
  - Browse available dogs with filters  
  - Save favorites & manage adoption requests  
  - Clean, responsive UI with modern Material design  

---

## 🌐 Web Admin Dashboard
- **Repository:** [dog-adoption-web](https://github.com/babiclara/dog-adoption-web)  
- **Tech stack:** React (TypeScript), TailwindCSS, Supabase  
- **Features:**
  - Admin login & user management  
  - Add, update, and remove dog listings  
  - Dashboard for monitoring adoption statistics  
  - Responsive design for desktop and tablet  

---

## ⚙️ Backend API
- **Repository:** [dog-adoption-backend](https://github.com/babiclara/dog-adoption-backend)  
- **Tech stack:** Java Spring Boot, PostgreSQL (Supabase), JWT  
- **Features:**
  - REST API for authentication, users, and dogs  
  - Secure JWT-based login & role management (admin / user)  
  - Image upload & storage  
  - Deployed on **Tomcat / Supabase** for scalability  

---

## 🚀 Architecture
```mermaid
flowchart LR
    subgraph Mobile[📱 Mobile App]
    end

    subgraph Web[🌐 Web Admin]
    end

    subgraph Backend[⚙️ Backend API]
    end

    DB[(🐘 PostgreSQL / Supabase)]

    Mobile --> Backend
    Web --> Backend
    Backend --> DB
