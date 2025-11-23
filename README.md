Here is a **perfect, clean, professional README.md** for your **SafeSpace – Women Safety & Emergency Alert System** including all screenshots you provided (I inserted placeholder paths — you can replace them with GitHub image URLs after pushing).

---

# 🚨 SafeSpace – Women Safety & Emergency Alert System

*A MERN-Stack Emergency Response Platform with Real-Time SOS Alerts*

---

## 📌 Overview

SafeSpace is a full-stack safety application designed to help users send instant emergency alerts (SOS) with **live location**, **email notifications**, and **emergency contact management**.
Built using the **MERN Stack**, it ensures fast response, secure authentication, and seamless UI/UX.

---

## 🚀 Features

### 🔐 Authentication

* User Registration with email
* Secure Login with JWT
* Protected Routes

### 📇 Emergency Contacts

* Add, View, and Delete contacts
* Each contact includes **Name, Phone, Email**
* Stored securely in MongoDB

### 🚨 SOS Alerts

* Centre emergency button
* On tap:

  * User's GPS location is captured
  * Email alert is sent to all saved emergency contacts
  * Timestamp is logged locally in the UI

### 🗺 Live Location Map

* Google Maps view
* Route navigation
* Satellite/Map modes
* Real-time location tracking

---

## 🛠️ Tech Stack

### Frontend

* React
* Axios
* Google Maps API
* CSS / Inline UI Styling

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* Nodemailer (for email SOS alerts)
* JWT Authentication

---

## 📁 Project Structure

```
SafeSpace/
├── backend/
│   ├── routes/
│   ├── models/
│   ├── config/
│   ├── server.js
│   └── .env      ❌ DO NOT COMMIT
│
└── frontend/
    ├── src/
    ├── components/
    └── .env      ❌ DO NOT COMMIT
```

---
Your screenshot section is **perfect** — only one small improvement is needed:

👉 **Right now, the description text appears on the SAME LINE as the image in GitHub.**
To fix that, you must add a **blank line** after each image tag.

Here is your entire corrected block, perfectly formatted for GitHub **README.md**:

---

## 🖼️ Screenshots

### **1️⃣ Register Screen**

<img width="624" height="281" alt="image" src="https://github.com/user-attachments/assets/2c808c62-752d-4271-8629-ab31ca1aa0fe" />

This screen allows new users to create an account by entering their name, email, and password. The UI follows a glassmorphism card design for a clean and modern onboarding experience.

---

### **2️⃣ Login Screen**

<img width="624" height="280" alt="image" src="https://github.com/user-attachments/assets/7c026271-0593-4916-b266-bbc0e12c8313" />

Users can securely log in using their registered email and password. The interface includes a gradient login button and a link to navigate to the registration page.

---

### **3️⃣ Dashboard**

<img width="624" height="280" alt="image" src="https://github.com/user-attachments/assets/dc248094-426b-4930-b22b-753163886be0" />

After login, the dashboard provides quick access to the main features — Home, Contacts, SOS, and Map. Each option is displayed as a large interactive tile for easy navigation.

---

### **4️⃣ Emergency Contacts Screen**

<img width="624" height="285" alt="image" src="https://github.com/user-attachments/assets/32b04cbd-5867-45bd-abc5-ad84dc9ccd54" />

Users can add new emergency contacts including Name, Phone Number, and Email. Saved contacts are displayed in a list format with an option to delete them if needed.

---

### **5️⃣ SOS Alert Screen**

<img width="624" height="280" alt="image" src="https://github.com/user-attachments/assets/3d2df0ba-7810-4efe-a2d3-e865da2cc3f2" />

This interface contains a central SOS button that sends an emergency email alert along with the user's live location. A timestamp log is shown under the button displaying past SOS triggers.

---

### **6️⃣ Live Map Screen**

<img width="624" height="282" alt="image" src="https://github.com/user-attachments/assets/e5f4c61d-3e80-4449-9d46-0b0eef09a690" />

The map screen uses Google Maps to display the user’s current location and allows route navigation. The top search bar helps users locate destinations, and real-time movement is supported.

---


## ⚙️ Installation & Setup

### 1️⃣ Clone the repo

```bash
git clone https://github.com/your-username/SafeSpace.git
```

### 2️⃣ Backend Setup

```bash
cd backend
npm install
```

Create `.env`

```
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_secret
EMAIL_USER=your_email
EMAIL_PASS=your_email_password_or_app_password
```

Start backend

```bash
npm run dev
```

### 3️⃣ Frontend Setup

```bash
cd frontend
npm install
```

Create `.env`

```
REACT_APP_API_URL=http://localhost:5000/api
REACT_APP_GOOGLE_MAPS_KEY=your_key
```

Start frontend

```bash
npm start
```

---

## 📬 SOS Email Alert Format

When SOS is triggered, the emergency contacts receive an email:

```
Subject: 🚨 SOS Alert – Immediate Help Needed!

Message:
User triggered an SOS alert.

Live Location:
https://www.google.com/maps?q=LAT,LNG

Please reach out immediately.
```

---

## 🔐 Security Notes

✔ `.env` files **must NEVER be pushed** to GitHub
✔ Use Gmail App Passwords for Nodemailer
✔ Ensure MongoDB IP whitelist is configured

---

## 🤝 Contributions

Pull requests are welcome!

---

## 📄 License

MIT License

---
