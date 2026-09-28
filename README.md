# study__buddy
AI StudyBuddy is an AI-powered learning assistance platform designed to
help students study smarter. It uses Generative AI to create summaries,
flashcards, quizzes, and personalized study plans from study materials.

## 👥 Team Details

  Role          Name
  ------------- -----------------
  Team ID       SWTID-2026-4525
  Team Size     5
  Team Leader   TAMILSELVAN P
  Team Member   SANJAY K
  Team Member   SUJITH R
  Team Member   ROSEMARY S
  Team Member   KAVINKUMAR P

## 🎯 Project Objective

The main objective of AI StudyBuddy is to provide students with a
centralized platform for managing study materials and generating useful
learning resources with the help of AI.

Students can upload or enter study content and use AI to:

-   Generate concise summaries
-   Create flashcards
-   Generate multiple-choice quizzes
-   Create personalized study plans
-   Save generated learning resources for future reference

## ✨ Key Features

-   🔐 JWT-based user authentication
-   👤 Student and Admin roles
-   📄 Study material upload and management
-   📝 AI-generated summaries
-   🃏 AI-generated flashcards
-   ❓ AI-generated quizzes
-   📅 Personalized AI study plans
-   🗄️ MongoDB database
-   🔒 Password protection using bcryptjs
-   🛡️ Role-Based Access Control (RBAC)
-   🤖 Google Gemini AI integration
-   🔌 RESTful API architecture

## 🛠️ Technologies Used

-   **Frontend:** React.js
-   **Backend:** Node.js, Express.js
-   **Database:** MongoDB
-   **ODM:** Mongoose
-   **AI:** Google Gemini API
-   **Authentication:** JWT
-   **Password Security:** bcryptjs
-   **File Upload:** Multer
-   **API Testing:** Postman / Thunder Client
-   **Development Tool:** Visual Studio Code

## 🏗️ Project Architecture

The project follows a modular RESTful architecture and MVC pattern.

``` text
Client (React.js)
       ↓
Express.js Server
       ↓
Authentication Middleware (JWT)
       ↓
Routes / Controllers
       ↓
 ┌───────────────┬────────────────┐
 ↓               ↓                ↓
MongoDB       Gemini AI       File Upload
(Mongoose)       API            (Multer)
```

## 📂 Main Backend Structure

``` text
AI StudyBuddy/
│
├── index.js
├── package.json
├── .env
├── .gitignore
│
└── src/
    ├── middleware/
    │   ├── auth.js
    │   └── upload.js
    │
    ├── models/
    │   ├── User.js
    │   └── Material.js
    │
    └── utils/
        ├── db.js
        └── gemini.js
```

## ⚙️ Installation

### 1. Clone the repository

``` bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd AI-StudyBuddy
```

### 2. Install dependencies

``` bash
npm install
```

The project uses packages such as:

``` bash
npm install express mongoose bcryptjs jsonwebtoken cors dotenv multer @google/genai
```

For development:

``` bash
npm install --save-dev nodemon
```

### 3. Configure environment variables

Create a `.env` file in the project root:

``` env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key
```

> **Important:** Do not upload your real `.env` file or API keys to
> GitHub.

## ▶️ Run the Project

Start the backend server:

``` bash
npm start
```

The backend connects to MongoDB and starts accepting API requests.

## 🔗 Main API Endpoints

  Feature                 Method   Endpoint
  ----------------------- -------- --------------------------------
  User Registration       POST     `/api/auth/register`
  User Login              POST     `/api/auth/login`
  Upload Study Material   POST     `/api/material/upload`
  Generate Summary        POST     `/api/materials/:id/summarize`
  Generate Flashcards     POST     `/api/ai/flashcards`
  Generate Quiz           POST     `/api/ai/quiz`
  Generate Study Plan     POST     `/api/ai/study-plan`

## 👨‍🎓 Student Functions

Students can:

1.  Register and log in.
2.  Upload study materials.
3.  Generate AI summaries.
4.  Create flashcards.
5.  Generate quizzes.
6.  Generate personalized study plans.
7.  View and manage previously generated resources.

## 👨‍💼 Admin Functions

Administrators can:

-   Manage registered users
-   Monitor application activity
-   Monitor AI service usage
-   Review system logs
-   Maintain system integrity
-   Handle user-related issues

## 🔐 Security

AI StudyBuddy uses:

-   JWT authentication for protected routes
-   bcryptjs for password protection
-   Role-Based Access Control (RBAC)
-   Environment variables for sensitive configuration
-   Protected administrative APIs

## 📊 Database

MongoDB stores:

-   User information
-   Study materials
-   AI-generated summaries
-   Flashcards
-   Quizzes
-   Study plans

Mongoose is used for schema definitions, validation, and database
operations.

## 🚀 Project Outcome

AI StudyBuddy reduces the manual effort required to prepare study notes,
revision questions, and study schedules. By combining AI with a secure
backend, the project provides a centralized and personalized learning
support platform for students.

## 👥 Team

**Team ID:** SWTID-2026-4525

**Team Leader:** TAMILSELVAN P

**Team Members:** - SANJAY K - SUJITH R - ROSEMARY S - KAVINKUMAR P

------------------------------------------------------------------------

### 📌 Project Name

**AI StudyBuddy -- AI Assistant for Smarter Learning and Study Support**

> Developed as a college project by Team SWTID-2026-4525.
