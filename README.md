# 📘 VidyaSathi — AI Tutor for Every Indian Student

VidyaSathi is an AI-powered educational web application designed to support Maharashtra Board (SSC 10th & HSC 12th) students. It provides interactive learning through AI chat, quizzes, dashboards, and study planning tools to enhance self-study and performance tracking. 

---

## 🚀 Features

* 🤖 **AI Chat Tutor** – Ask subject-specific questions with real-time streaming responses
* 🎤 **Voice Support** – Speech-to-text input and text-to-speech output (English & Hindi)
* 📝 **Quiz System** – Chapter-wise quizzes and timed mock tests with explanations
* 📊 **Dashboard Analytics** – Track performance, streaks, weak areas, and progress
* 🔖 **Bookmarks Hub** – Save and manage important answers for revision
* 📅 **Study Planner** – Organize tasks with priority, deadlines, and completion tracking
* 📚 **Textbook Integration** – AI responses based on textbook content

---

## 🛠️ Tech Stack

**Frontend**

* React 18
* TypeScript
* Vite
* Tailwind CSS
* shadcn/ui + Radix UI

**Libraries & Tools**

* Framer Motion (animations)
* Recharts (data visualization)
* React Router (routing)
* React Query (data handling)
* Lucide React (icons)

**Backend**

* Lovable Cloud Functions
* Database integration for AI and textbook retrieval

---

## 📁 Project Structure

```
src/
 ├── pages/
 │   ├── Chat.tsx
 │   ├── Quiz.tsx
 │   ├── Dashboard.tsx
 │   ├── Bookmarks.tsx
 │   └── ...
 ├── components/
 │   └── VoiceInput.tsx
 ├── lib/
 │   ├── studyPlanner.ts
 │   └── quizAttempts.ts
 ├── App.tsx
 └── main.tsx
```

---

## 🔄 How It Works

### AI Chat Flow

* User inputs question (text or voice)
* Request sent to backend with class & subject
* Backend retrieves textbook context + generates response
* Streaming response displayed in real-time

### Quiz Flow

* User selects chapter or mock test
* App tracks score, timer, and answers
* Results saved locally for dashboard analysis

### Dashboard

* Aggregates:

  * Quiz attempts
  * Bookmarks
  * Study tasks
  * Chat activity
* Displays insights like average score, weak subjects, and streaks

---

## 💾 Data Storage

* **localStorage** → quiz data, bookmarks, study planner, chat history
* **Backend** → AI responses, textbook data, caching

---

## ⚙️ Installation & Setup

```bash
# Install dependencies
npm install

# Run development server
npm run dev
```

## 🔗 Live Demo

👉 [https://your-demo-link.com](https://your-demo-link.com)

---

## 🔐 Environment Variables

Create a `.env` file in the root directory:

```env
VITE_SUPABASE_PROJECT_ID="your_project_id"
VITE_SUPABASE_PUBLISHABLE_KEY="your_publishable_key"
VITE_SUPABASE_URL="your_supabase_url"
```

## 🌟 Future Improvements

* Sync student data across devices (move to backend)
* Export reports and analytics
* Role-based teacher dashboard
* Improve voice feature compatibility
* Add automated testing

---

## 📌 Quick Summary

VidyaSathi is a modern AI-based learning platform combining interactive tutoring, quizzes, analytics, and planning tools to help students study smarter and track their academic progress effectively. 
