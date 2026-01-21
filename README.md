# 🚀 FLEDGE — Smart Quiz Builder & Performance Prediction Platform

FLEDGE is a full-stack smart learning platform that allows users to **create quizzes**, **share them via QR codes**, **let students solve quizzes on any device**, and **instantly view results**.  
It also includes an **AI-powered performance prediction system** using Machine Learning.

---

## 📌 Key Features

### 🔐 Authentication System
- **Login**
- **Signup**
- **Forgot Password**
- Authentication is done using **Email + CNIC matching**
- User session maintained via **Local Storage**
- User details fetched securely from **Supabase Database**

---

### 🧠 Quiz Management System
#### 👨‍🏫 Quiz Creator (User)
- Create quizzes with:
  - Multiple questions
  - Multiple options
  - Correct answers
  - Timer
- Generate **unique quiz links**
- Generate **QR Code** for each quiz
- View all created quizzes
- View quiz results
- **Delete quizzes** anytime

#### 🎓 Student (Quiz Solver)
- Solve quizzes using:
  - Direct quiz link
  - **QR Code scan on another device**
- Timer-based quiz solving
- Instant result after submission
- Auto evaluation of answers

---

### 📊 Instant Results & Analytics
- Automatic score calculation
- Result shown immediately after quiz completion
- All quiz attempts stored in database
- User can view:
  - Quiz history
  - Student results
  - Performance summaries

---

### 🤖 Student Performance Prediction (Machine Learning)
- Predict student performance based on:
  - Study hours
  - Attendance
  - Previous scores
  - Other academic features
- Backend built using **Flask (Python)**
- Machine Learning model used for prediction
- Frontend communicates with Flask API
- Prediction results shown instantly

---

## 🧱 Tech Stack

### 🌐 Frontend
- **Next.js (App Router)**
- **React**
- **TypeScript**
- **Tailwind CSS**
- **QR Code Generation**
- **Client-side Routing**

### 🔙 Backend
- **Flask (Python)**
- REST APIs for ML prediction
- Model trained on student performance dataset

### 🗄️ Database
- **Supabase**
- Tables include:
  - `app_users`
  - `quizzes`
  - `questions`
  - `quiz_attempts`
  - `predictions`

### 🧠 Machine Learning
- Scikit-learn
- Pandas
- NumPy
- Trained model served via Flask

---

## 📂 Project Structure

FLEDGE/
│
├── app/
│ ├── login/
│ ├── signup/
│ ├── forgot/
│ ├── quiz/
│ ├── prediction/
│ ├── page.tsx
│ ├── layout.tsx
│
├── backend/
│ ├── app.py
│ ├── requirements.txt
│ ├── student1.csv
│
├── public/
│ ├── images/
│
├── README.md
├── package.json
├── tsconfig.json
└── .gitignore


---

## 🧩 How It Works

1. User signs up using **Email + CNIC**
2. User logs in and session is stored locally
3. User creates a quiz
4. Quiz link & QR code are generated
5. Student scans QR or opens link
6. Student solves quiz
7. Result shown instantly
8. Quiz data saved in database
9. User can view or delete quiz
10. User can predict performance using ML model

---


