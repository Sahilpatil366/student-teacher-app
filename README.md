# 🎓 EduBook - Smart Appointment Scheduling System

A smart, responsive, and user-friendly web application designed to simplify the process of scheduling meetings between students and teachers. EduBook eliminates manual coordination, providing a seamless digital experience for booking, managing, and tracking appointments with real-time updates.

## 🚀 Project Overview

EduBook bridges the communication gap in educational institutions by providing an organized scheduling platform. Users interact with the system through three distinct roles: **Admin, Teacher, and Student**. By utilizing Firebase for secure authentication and real-time database management, EduBook ensures that appointment requests, approvals, and user registrations are handled instantly and securely.

## ✨ Features

### 👤 Advanced Role-Based Authentication
* **Three User Roles:** Dedicated access for Admins, Teachers, and Students.
* **Admin Approval Gateway:** Student accounts are placed in a "Pending" state upon registration and require Admin activation to log in.
* **Smart Routing:** Users are automatically redirected to their specific dashboards upon login.
* **Robust Security:** Enforced lowercase email formatting to prevent database mismatch errors, alongside a smart "Show/Hide" password toggle for better UX.

### 📅 Real-Time Appointment Management
* **Student Dashboard:** Search for teachers, request appointment slots, and track status (Pending, Approved, Declined).
* **Teacher Dashboard:** View incoming requests and approve or decline them with a single click.
* **Instant Synchronization:** Powered by Firebase Firestore `onSnapshot` listeners, the UI updates automatically without needing a page refresh.

### 🛡️ Administrative Control
* **User Management:** Admins can view total user counts, delete accounts, and approve pending student registrations.
* **Teacher Onboarding:** Admins can securely generate and register new teacher accounts directly from the dashboard.

### 🎨 Modern UI/UX Design
* **Clean & Responsive:** Built with a mobile-friendly layout and the modern 'Inter' typeface.
* **Smooth Interactions:** Features invisible CSS bridges for flawless dropdown hover effects, dynamic form validation, and clean notification popups.

## 🛠️ Tech Stack

**💻 Frontend:**
* HTML5
* CSS3 (Custom responsive layouts, Flexbox, CSS Grid)
* Vanilla JavaScript (DOM manipulation, Event Listeners, Smart Routing)

**☁️ Backend / Database (Firebase):**
* Firebase Authentication (Email & Password)
* Firebase Cloud Firestore (NoSQL Real-time Database)

## 📂 Project Structure

\`\`\`text
edubook/
│
├── css/
│   ├── home.css
│   ├── login.css
│   ├── register.css
│   └── dashboard.css
│
├── js/
│   └── script.js          # Contains Firebase config, Auth logic, and Dashboard functions
│
├── index.html             # Landing Page
├── login.html             # Login Portal
├── register.html          # Registration Portal
├── admin-dashboard.html   # Admin Control Panel
├── teacher-dashboard.html # Teacher Schedule Manager
└── dashboard.html         # Student Booking Portal
\`\`\`

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
\`\`\`bash
git clone https://github.com/Sahilpatil366/student-teacher-app.git
\`\`\`

### 2️⃣ Navigate to the Project Folder
\`\`\`bash
cd student-teacher-app
\`\`\`

### 3️⃣ Firebase Setup (Crucial)
1. Go to the [Firebase Console](https://console.firebase.google.com/).
2. Create a new project.
3. Go to **Authentication** and enable **Email/Password** sign-in.
4. Go to **Firestore Database** and create a database (Start in Test Mode for development).
5. Go to Project Settings, register your web app, and copy the `firebaseConfig` object.
6. Open `js/script.js` and replace the existing `firebaseConfig` with your own keys.

### 4️⃣ Run the App
Simply open `index.html` in your web browser or use a local server like VS Code's "Live Server" extension.

## 🌐 Future Enhancements

* 📧 **Email Notifications:** Trigger automated emails when an appointment is approved or declined.
* 📅 **Calendar Integration:** Sync approved appointments directly to Google Calendar.
* 💬 **In-App Chat:** Allow students and teachers to message each other before a meeting.
* 📱 **Native Mobile App:** Build an iOS/Android version using React Native or Flutter.

## 🤝 Contributing

Contributions are welcome! If you'd like to improve this project:
1. Fork the repository
2. Create a new branch (`git checkout -b feature/AmazingFeature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
5. Push to the branch (`git push origin feature/AmazingFeature`)
6. Submit a Pull Request

##
