# 🏝️ Bali Currency Tracker

A beautiful, real-time money tracking app for your Bali trip!

## Features
- 💰 Track IDR balance with INR conversion
- 📊 Categorized spending with analytics
- 📱 Mobile-friendly design
- 🎨 Beautiful gradient UI

🎯 **Usage**

Set Your Budget - Use the 💰 button to set your initial IDR balance and exchange rate
Track Spending - Record expenses with categories and descriptions
View Analytics - Check the 📊 button for spending breakdowns
Convert Currency - Use the quick converter for real-time IDR to INR conversion****

## Live Demo
[View App](https://kriti-nigam.github.io/bali-currency-tracker/)

## Tech Stack
- Vanilla JavaScript
- Firebase Firestore
- CSS Gradients & Animations
- Canvas API for charts

🛠️ **Setup Instructions**
**Prerequisites**

A Firebase account
Basic knowledge of web hosting

1. Clone the Repository
bashgit clone https://github.com/yourusername/bali-money-tracker.git
cd bali-money-tracker
2. Set Up Firebase

Go to Firebase Console
Create a new project
Enable Firestore Database
Set up Firestore security rules:
javascriptrules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /users/{userId} {
      allow read, write: if true;
    }
    match /{document=**} {
      allow read, write: if false;
    }
  }
}


3. Configure Firebase

Go to Project Settings → General → Your apps
Add a web app and copy the config
Replace the Firebase configuration in the HTML file:
javascriptconst firebaseConfig = {
  apiKey: "your-api-key",
  authDomain: "your-project.firebaseapp.com",
  projectId: "your-project-id",
  storageBucket: "your-project.appspot.com",
  messagingSenderId: "123456789",
  appId: "your-app-id"
};


4. Deploy

Upload the HTML file to any web hosting service
Or use Firebase Hosting for easy deployment

