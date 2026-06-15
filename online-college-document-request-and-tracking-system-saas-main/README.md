# 🎓 CampusLedger – Smart College Document Request & Tracking System

A **full-stack MERN application** that digitalizes college document workflows, reducing manual paperwork and improving request visibility through automated approvals and tracking.

## ⚡ Problem & Solution

**Problem:** Students navigate manual paperwork, multiple department visits, and lack visibility into document requests.

**Solution:** Centralized digital platform with role-based workflows, real-time tracking, and automated notifications.

---

## ✨ Key Features

| Feature | Benefit |
|---------|---------|
| **Role-Based Access Control** | Student, Admin, HOD, Principal dashboards |
| **Multi-Level Approval Workflow** | Structured request lifecycle management |
| **Real-Time Request Tracking** | Students monitor status, comments, history |
| **Automated Email Notifications** | Instant updates at each workflow stage |
| **Secure Document Distribution** | Protected PDF uploads & downloads |
| **Eligibility Validation** | Automated institutional rule enforcement |

---

## 🛠 Tech Stack

**Frontend:** React 19 | React Router | Axios | Bootstrap 5 | Formik/Yup

**Backend:** Node.js | Express.js | MongoDB | Mongoose

**Security:** JWT | bcrypt | Helmet | CORS | Rate Limiting

**Infrastructure:** Docker | Docker Compose | NGINX | GitHub Actions | Render

**Services:** SendGrid API | Cloudinary | Morgan/Winston Logging

---

## 🏗 System Architecture

```
React Frontend → Axios HTTP → Express REST API → MongoDB
                                    ↓
                    ┌───────────────┼───────────────┐
                    ↓               ↓               ↓
              Cloudinary      Email Service      Logs
```

---

## 🚀 Quick Start

### Backend
```bash
cd backend
npm install
npm run dev
```

### Frontend
```bash
cd frontend
npm install
npm start
```

### Docker
```bash
docker-compose up --build
```

---

## 📁 Project Structure

```
├── backend/
│   ├── controllers/    (Business logic)
│   ├── models/         (MongoDB schemas)
│   ├── routes/         (API endpoints)
│   ├── middleware/     (Auth, validation)
│   ├── services/       (Email, notifications)
│   └── server.js
├── frontend/
│   ├── src/
│   │   ├── pages/      (Student & Admin portals)
│   │   ├── components/ (Reusable UI)
│   │   └── services/   (API integration)
│   └── package.json
└── docker-compose.yml
```

---

## 🌐 Core API Endpoints

```
POST   /api/auth/register       - Student registration
POST   /api/auth/login          - Authentication
GET    /api/users/me            - Current user profile
POST   /api/requests            - Create document request
GET    /api/requests            - List requests (role-based)
PUT    /api/requests/:id        - Update request status
POST   /api/documents           - Upload documents (admin)
GET    /api/documents/:id       - Download documents
```

---

## 🔒 Security Highlights

✅ JWT-based authentication with secure token validation  
✅ Password hashing using bcrypt  
✅ Role-based authorization (RBAC)  
✅ Helmet security headers  
✅ CORS protection  
✅ Rate limiting on auth endpoints  
✅ Secure document access links  

---

## 📊 Workflow

```
Student → Submit Request → Admin Review → HOD Approval → 
Principal Approval → Document Generation → Issuance → Download
```

Each stage triggers automated notifications and timeline updates.

---

## 🔮 Future Enhancements

- Digital signature integration
- SMS notifications
- Analytics dashboard
- Mobile application
- ERP integration
- AI-powered document validation

---

## 📦 Environment Variables

**Backend:** `MONGO_URI`, `JWT_SECRET`, `PORT`, `EMAIL_USER`, `EMAIL_PASS`, `CLOUDINARY_*`

**Frontend:** `REACT_APP_API_URL`

---

## 📈 Deployment

- **Docker:** Containerized multi-service deployment
- **GitHub Actions:** Automated CI/CD pipeline
- **Render:** Production hosting with health checks

---

## 👩‍💻 Author

**Subashree S**  


---

**[View Repository](https://github.com/Subashree-selvaraj/online-college-document-request-and-tracking-system-saas)**
