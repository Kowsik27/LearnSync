# EduLMS - A Learning Management System

A full-stack **Learning Management System** built with a focus on clean backend architecture, secure authentication, and real-world workflows. This project demonstrates practical experience with REST APIs, authentication, and deployment.

---

## 🚀 Live Demo  
👉 https://lms-frontend-znsz.onrender.com/


# EduLMS – Complete Feature List

EduLMS is a full-stack Learning Management System designed to manage courses, users, assessments, and payments with a secure, role-based architecture.

---

## 1. Role-Based Access & Dashboards

EduLMS supports three primary user roles, each with a dedicated dashboard:

### Admin Dashboard

* Manage users (students and instructors)
* Manage courses and quizzes
* System configuration and settings
* View analytics and reports
* Handle approval workflows

### Instructor Dashboard

* Create and manage courses and quizzes
* Track student progress and performance
* Submit courses and content for admin approval
* View enrolled students

### Student Dashboard

* Browse and enroll in courses
* View learning progress and completion status
* Access course materials
* Submit assignments

---

## 2. Course Management

* Create courses with a modular hierarchy (Modules → Lessons → Topics)
* Support for multimedia content (videos, PDFs, images, embedded links)
* Admin approval workflow before course publication
* Course categorization and tagging for better discoverability

---

## 3. Assessment & Evaluation

### Quizzes

* Multiple-choice questions
* True/False questions
* Short answer questions
* Automatic grading with instant results

### Assignments

* File submission system (PDF, DOC, images)
* Manual grading by instructors
* Feedback and commenting system

---

## 4. Authentication & Security

* OTP-based authentication system

  * OTP signup and registration
  * OTP login
  * OTP-based password reset
  * Email verification
* Secure session management
* Role-based access control across the platform

---

## 5. Communication & Notifications

* Course and system announcements by instructors and admins
* Real-time notifications using Socket.IO

  * New content updates
  * Approval status changes
  * Assignment deadlines
* Email notifications using Nodemailer

  * OTP delivery
  * Enrollment confirmations
  * Course and system updates

---

## 6. Admin Approval System

* Instructor account approval and rejection
* Course approval before publication
* Optional approval for quizzes and assessments
* Centralized approval dashboard with:

  * Pending courses (with preview support)
  * Pending instructor registrations
  * Pending quizzes/content
* Quick approve/reject actions with comments

---

## 7. Progress Tracking & Analytics

### Student Progress Tracking

* Visual progress bars
* Course completion percentages

### Admin Analytics

* Enrollment statistics
* Course popularity metrics
* Revenue reports for paid courses
* User engagement analytics

### Instructor Analytics

* Student progress reports
* Quiz performance analysis
* Course completion rates

---

## 8. Payment & Enrollment

### Course Enrollment

* Free courses with instant enrollment
* Paid courses with Razorpay integration
* One-time payment support

### Razorpay Integration

* Secure payment processing
* Payment success and failure handling
* Refund management
* Automated payment notifications

### Certificate Generation

* Automated PDF certificate generation upon course completion
* Customizable certificate templates
* Certificate verification system

---

## 9. Technical Specifications

* **Frontend:** React.js
* **Backend:** Node.js with Express.js
* **Database:** MongoDB
* **Real-Time Communication:** Socket.IO
* **Email Service:** Nodemailer
* **Payment Gateway:** Razorpay API
* **File Storage:** Cloudinary
* **PDF Generation:** PDFKit
* **Hosting:** Render
* **Responsive Design:** Fully mobile-friendly interface



## 📂 Project Structure

```
server/
├── controllers/
├── routes/
├── models/
├── middleware/
├── utils/
├── config/
└── index.js

client/
├── components/
├── pages/
└── services/
```

---

## 🔐 Authentication Flow

1. User registers or logs in
2. Passwords are securely hashed using bcrypt
3. JWT is issued and stored on the client
4. Protected routes are accessed using auth middleware
5. Forgot-password flow handled via secure email link / OTP

**Example:**

> A tutor logs in and accesses protected course and profile APIs using JWT authentication.

---

## 🌱 Environment Variables

```
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
EMAIL_USER=your_email
EMAIL_PASS=your_email_password
CLIENT_URL=frontend_url
```

---

## ▶️ Run Locally

**Backend**

```
cd server
npm install
npm start
```

**Frontend**

```
cd client
npm install
npm run dev
```

---

## 🚀 Deployment

* Backend deployed on **Render**
* Frontend deployed separately
* CORS & port binding configured for production

---

## 📌 What I Learned

* Designing scalable REST APIs
* Implementing secure authentication systems
* Backend error handling & middleware patterns
* Real-world deployment and environment management
* Working with industry tools like JIRA & Postman

---

## 👨‍💻 Author

**Mohith**
CSE 2K27 | Backend & DSA Enthusiast

---

⭐ If you find this project useful, consider giving it a star!
