LMS Micro-Certification Portal

A micro-certification platform where students can attempt small quizzes (MCQs), view results instantly, and download a personalized certificate with their name and score.

This project is a mini version of a certification engine that can later be integrated into the AGH LMS.

🚀 Features

🔑 User Authentication: Login/Register before taking quizzes.

📝 Quiz Interface: Question-by-question navigation with multiple-choice questions (MCQs).

⚡ Instant Results: Automatic score calculation with pass/fail status.

📄 Certificate Generation: Auto-generated PDF certificate with student’s name, quiz title, and score.

💾 Database Integration: Stores users, questions, and results.

🌐 Deployment: Fully deployed on Vercel (frontend + backend).

🛠️ Tech Stack
Frontend (React)

React + React Router (quiz flow and navigation)

Axios (API integration)

TailwindCSS / Bootstrap (UI styling)

Backend (Node.js + Express)

REST APIs for quiz retrieval, result calculation, and certificate generation

PDF generation using pdfkit / jspdf

Database

MongoDB (Mongoose) / SQL alternative

Schema for Users, Questions, and Results

📂 Database Schema
Users
{
  "id": "ObjectId",
  "name": "String",
  "email": "String",
  "password": "String (hashed)"
}

Questions
{
  "id": "ObjectId",
  "quizId": "String",
  "questionText": "String",
  "options": ["String"],
  "correctAnswer": "String"
}

Results
{
  "id": "ObjectId",
  "userId": "ObjectId",
  "quizId": "String",
  "score": "Number",
  "date": "Date"
}

📌 Acceptance Criteria

✅ Users can log in/register before taking a quiz.
✅ Quiz shows MCQs one by one with navigation.
✅ Instant result screen with score and pass/fail status.
✅ PDF Certificate auto-generated & downloadable.
✅ All data stored in MongoDB/SQL database.
✅ Fully deployed on Vercel (frontend + backend).

⚙️ Setup Instructions
1. Clone Repo
git clone https://github.com/your-username/lms-micro-certification.git
cd lms-micro-certification

2. Backend Setup
cd backend
npm install


Create a .env file:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key


Run server:

npm run dev

3. Frontend Setup
cd frontend
npm install
npm start

📄 Certificate Sample

(Include a screenshot of your generated certificate here)

🌐 Deployment

Frontend deployed on Vercel: Live Link

Backend deployed on Vercel: API Link

🖼️ Screenshots

Login/Register Screen

Quiz Interface

Result Page

Certificate

(Add actual screenshots here once project is running)

📊 Evaluation Metrics

Functionality (40%) – Quiz flow, result calculation, certificate generation

Code Quality (20%) – Clean APIs, modular structure, error handling

UI/UX (15%) – Smooth quiz navigation, clear results, professional certificate design

Database Design (10%) – Well-structured schema with relations

Deployment (10%) – Fully functional on Vercel

Innovation (5%) – Extra features (timed quizzes, leaderboard, shareable certificates)

✨ Extra Features (Optional)

⏱️ Timed quizzes

🏆 Leaderboard for top scorers

🔗 Shareable certificates via unique links

📜 License

This project is for educational purposes only.
