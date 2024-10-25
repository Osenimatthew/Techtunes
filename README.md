# TechTunes - Music Streaming Website

## Overview
**TechTunes** is a music streaming website built using HTML, CSS, JavaScript, Firebase, and the Jamendo API. The platform allows users to browse songs, play music, save songs to playlists, and create their own playlists. Firebase is used for user authentication and database management.

## Features
- User authentication (signup/login)
- Music streaming via the Jamendo API
- Create and manage personal playlists
- Responsive design for all devices

## Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Firebase (for authentication and database)
- **Music API:** Jamendo API
- **Version Control:** GitHub

---

## Setup Guide

### Prerequisites
Before setting up the project, ensure you have the following installed on your machine:
- A **GitHub** account
- A **Firebase** account: Set up at [Firebase](https://firebase.google.com/)
- A **Jamendo API** account: Get API access from [Jamendo Developers](https://developers.jamendo.com/)

---

### 1. Clone the Repository
Clone the TechTunes repository from GitHub using the following command:

```bash
git clone https://github.com/yourusername/techtunes.git
cd techtunes
```

### 2. Firebase Setup

#### a. Create a Firebase Project
1. Go to the [Firebase Console](https://console.firebase.google.com/).
2. Click **Add Project** and follow the steps to create a new project for TechTunes.
3. After the project is created, go to the **Authentication** section and enable **Email/Password Authentication**.
4. In the **Firestore Database**, create a database to store users' playlist data.

#### b. Add Firebase SDK to the Project
1. In the Firebase Console, click on **Project Settings**.
2. Scroll down to **Your Apps** and select **Add Firebase to your Web App**.
3. Copy the Firebase SDK config (it will look like the code below).

```javascript
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};
```

4. Paste the config in your project's `firebase.js` file (or wherever appropriate).

---

### 4. Jamendo API Setup

#### a. Get Deezer API Access
1. Create a Deezer developer account at [Jamendo Developers](https://developers.jamendo.com/).
2. Get an API key to use for accessing music data.

#### b. Update API in Your Code
Add your **Jamendo API key** to the relevant part of your JavaScript code:

```javascript
const deezerAPIKey = "YOUR_JAMENDO_API_KEY";
```

Use the API key when making requests to Jamendo to fetch songs, albums, and playlists.

---

### 5. Run the Project Locally

After completing the setup, run the project locally by opening the `index.html` file in your browser.

Alternatively, you can use a local server for development:

This will open the project in your default browser and refresh automatically on file changes.

---

### 6. Deploying to Firebase

To deploy the project on Firebase Hosting:
1. Install Firebase tools:

   ```bash
   npm install -g firebase-tools
   ```

2. Log in to Firebase:

   ```bash
   firebase login
   ```

3. Initialize Firebase in your project directory:

   ```bash
   firebase init
   ```

4. Deploy the project:

   ```bash
   firebase deploy
   ```

---

## Next Steps
- Continue adding more features such as advanced playlist management.
- Improve the user interface for a better music streaming experience.
- Add social sharing or other interactive features.

## Lessons Learned
- Working with the Jamendo API and managing API requests efficiently.
- Setting up Firebase for authentication and database management.
- Collaboration using GitHub and version control.

---


You can access this website using this link
 (https://osenimatthew.github.io/Techtunes/).
