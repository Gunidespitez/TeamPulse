# TeamPulse - AI Student Workload & Team Finder

## Project Description
TeamPulse is a full-stack student platform that **prevents burnout** by tracking workload (🟢🟡🟠🔴), **matching teammates** (college + skills + availability), and **AI coaching** ("Drop ML - overload risk!"). Hackathon-ready MVP!

**## Tech Stack (12 Technologies)**
**Frontend:** HTML5/CSS3/Vanilla JS (ES6+)  
**Backend:** Firebase Firestore v10 + Auth  
**AI/ML:** Google Gemini 1.5 Flash API  
**Charts:** Custom SVG Rings + CSS Gradients  
**Deployment:** Firebase Hosting (Live)  
**Queries:** Firestore Compound Indexes  
**Responsive:** CSS Grid/Flexbox (Mobile-first)  
**Storage:** 1MB/doc limit optimized

**## Features (9 Core + Polish)**
- **Firebase Auth** - Email signup/login (Task 2)
- **Profile Mgmt** - Skills/college/workload (Task 3)  
- **Smart Matching** - Same college + skills + 🟢🟡 (Task 4)
- **AI Chatbot** - Profile-aware advice ("Perfect Web Dev match!") (Task 5)
- **Burnout Dashboard** - Home AI recs (Task 6)
- **Task Manager** - Add/remove → auto color update (Task 7)
- **Real-time Sync** - Tasks/colors across devices
- **Mobile Responsive** - Perfect iPhone/Android UX
- **Firestore Structure** - users/{uid}/ + teams/{teamId}/

**## Installation (2 Minutes)**

1. console.firebase.google.com → New project → Enable Auth/Firestore
2. Copy config → Paste in index.html <script>
3. makersuite.google.com/app/apikey → Gemini key → Paste GEMINI_API_KEY
4. Live Server / python -m http.server 8000
5. firebase deploy → Live URL!

**##  System Architecture**
![Architecture Flowchart](flowchart.jpg)

**##  API Documentation** 
Firebase Authentication API v10.12.2
Used For: User login/signup, session management
Key Methods:

signInWithEmailAndPassword(email, password)

createUserWithEmailAndPassword(email, password)

onAuthStateChanged(callback)

signOut()

Firebase Firestore API v10.12.2
Used For: Real-time team data sync, task storage, heatmap generation
Key Methods:

getDoc(), setDoc(), updateDoc()

onSnapshot() for live updates

collection(), doc(), addDoc()
Collections: users, teams, tasks

**##Data structures:**
/users/{userId} → User profiles + workload
/teams/{teamId} → Team configs + members  
/tasks/{userId} → Individual task lists
**## 👥 Team Members**
- Anvita Dey
- Gunisha Kaur

**## 📄 License**
TeamPulse
© 2026 Anvita Dey & Gunisha Kaur
Licensed under MIT License

Permissions: Commercial use, modification, distribution, private use
Conditions: Include copyright notice in copies
Limitations: No liability, no warranty
undefined
