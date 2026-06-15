# 💊 DoseGuard – Smart Accessible Medication Management System

## 📌 Overview

**DoseGuard** is a smart medication management and caregiver assistance platform designed for **elderly and visually impaired individuals**. The application helps users manage daily medications through intelligent reminders, pill tracking, voice assistance, and caregiver notifications. It aims to improve medication adherence while providing an accessible and user-friendly interface.

## ✨ Features

* 📅 **Medication Dashboard**

  * Add, edit, and delete medications.
  * Schedule dose timings and frequencies.
  * Track pill stock and compartment location.

* ⏰ **Smart Dose Reminders**

  * Real-time medication alerts.
  * Snooze functionality for delayed intake.
  * Automatic missed-dose detection.

* 👨‍⚕️ **Caregiver Alert System**

  * Stores caregiver details.
  * Generates alerts for missed medications.
  * SMS notification integration (via Twilio backend).

* 📊 **Adherence Tracking**

  * Dynamic 7-day medication adherence chart.
  * Daily tracking of taken and missed doses.
  * Adherence statistics and trend visualization.

* 🎤 **Voice Interface**

  * Text-to-Speech (TTS) medication reminders.
  * Adjustable speech speed and volume.
  * Accessibility-focused voice interactions.

* ♿ **Accessibility Features**

  * High contrast mode.
  * Large text support.
  * Braille label support.
  * Screen-reader friendly interface.

* 💊 **Pillbox Status Monitoring**

  * Displays current pill stock.
  * Low-stock alerts.
  * Pill compartment management.

* 📱 **Responsive & Mobile Friendly**

  * Optimized for desktop and mobile devices.
  * Ready for Android deployment using Capacitor.

---

## 🛠️ Tech Stack

### Frontend

* React.js
* TypeScript
* Vite
* Tailwind CSS
* Framer Motion
* Lucide React Icons

### Backend

* Node.js
* Express.js
* Axios

### Database & Storage

* Local Storage (Current Version)
* Firebase Firestore (Planned Integration)

### Communication

* Twilio SMS API
* Browser Speech Synthesis API

### Mobile Deployment

* Capacitor
* Android Studio

---

## 🏗️ Project Architecture

```text
                +----------------------+
                |      User Login      |
                +----------+-----------+
                           |
                           v
              +-------------------------+
              |      Home Dashboard      |
              +----+-----+-----+--------+
                   |     |     |        
        +----------+     |     +------------+
        |                |                  |
        v                v                  v
+---------------+ +--------------+ +----------------+
| Medication    | | Voice         | | Caregiver      |
| Dashboard     | | Interface     | | Alert System   |
+-------+-------+ +------+--------+ +--------+-------+
        |                 |                  |
        +--------+--------+--------+---------+
                 |                 |
                 v                 v
         +-------------------------------+
         | Local Storage / Firebase (Future) |
         +-------------------------------+
                         |
                         v
                +----------------+
                | Twilio SMS API |
                +----------------+
```

---

## 🚀 Installation

### Clone the Repository

```bash
git clone https://github.com/Deepthish07/DoseGaurd.git
cd DoseGaurd
```

### Install Dependencies

```bash
npm install
```

### Run the Development Server

```bash
npm run dev
```

Open:

```
http://localhost:5173
```

### Build for Production

```bash
npm run build
```

---

## 📂 Project Structure

```text
src/
│
├── components/
│   ├── Dashboard.tsx
│   ├── MedicationCard.tsx
│   ├── CaregiverAlerts.tsx
│   ├── VoiceInterface.tsx
│   ├── Settings.tsx
│   ├── PillboxStatus.tsx
│   ├── HomePage.tsx
│   └── Header.tsx
│
├── contexts/
│   ├── AppContext.tsx
│   └── AccessibilityContext.tsx
│
├── App.tsx
├── main.tsx
└── index.css
```

---

## 🔄 Working Principle

1. User adds medication details, dosage, schedule, and caregiver information.
2. DoseGuard continuously monitors scheduled dose timings.
3. At medication time, the system generates an alert and voice reminder.
4. If the user marks the dose as taken, adherence statistics are updated.
5. If the dose remains unattended beyond the configured threshold, it is marked as **Missed**.
6. A caregiver alert is generated and an SMS notification can be sent through the backend.
7. Adherence charts and pill stock are automatically updated.

---

## 🎯 Future Enhancements

* Firebase Cloud Synchronization.
* IoT-enabled Smart Pillbox Integration.
* AI-based medication adherence prediction.
* OCR & Barcode scanning for medicine identification.
* GPS-based emergency caregiver notifications.
* Android and iOS native application deployment.

---

## 📸 Screenshots

> Add screenshots of:
>
> * Home Page
> * Medication Dashboard
> * Caregiver Alerts
> * Voice Interface
> * Accessibility Settings

---

## 👨‍💻 Author

**Deepthish**
B.Tech – Artificial Intelligence & Data Science

* GitHub: https://github.com/Deepthish07
* Project: DoseGuard – Smart Accessible Medication Management System

---

## 📜 License

This project is developed for **academic and research purposes** as part of a major project submission. It may be extended for healthcare and assistive technology applications in the future.
