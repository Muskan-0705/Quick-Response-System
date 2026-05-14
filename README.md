# Quick Response System

A React Native Emergency Response Application built with Expo. This app allows users to quickly send SOS alerts, share their live location, and notify emergency contacts in critical situations.

## 🚀 Features

*   **Authentication Flow:** Secure Login, Signup, and Splash screens using Firebase Authentication.
*   **SOS Alerts:** One-tap emergency alert system.
*   **Emergency Contacts:** Add and manage emergency contacts who will be notified during an SOS.
*   **Live Location Tracking:** Integrates `expo-location` and `react-native-maps` to capture and share real-time location.
*   **Cross-Platform Map Support:** Custom map implementations for both Web and Native platforms.
*   **SMS Integration:** Automatically send emergency text messages with location data using `expo-sms`.
*   **Voice Commands:** Hands-free emergency triggering using `expo-speech-recognition`.
*   **User Profile:** Manage user settings and profile information.

## 🛠️ Tech Stack

*   **Framework:** [React Native](https://reactnative.dev/)
*   **Platform:** [Expo](https://expo.dev/)
*   **Navigation:** [React Navigation](https://reactnavigation.org/) (Stack & Bottom Tabs)
*   **Backend & Authentication:** [Firebase](https://firebase.google.com/)
*   **Maps:** `react-native-maps`
*   **Hardware APIs:** `expo-location`, `expo-sms`, `expo-speech-recognition`, `expo-sensors`

## 📁 Project Structure

```
├── src/
│   ├── components/      # Reusable UI components
│   ├── context/         # React Context for global state management
│   ├── navigation/      # Navigation config (Stack/Tabs)
│   ├── screens/         # App screens (Home, Login, Map, etc.)
│   └── services/        # API calls, Firebase config, background tasks
├── assets/              # Images, fonts, and icons
├── App.js               # Application entry point
├── app.json             # Expo configuration
└── package.json         # Project dependencies
```

## ⚙️ Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone <https://github.com/Muskan-0705/Quick-Response-System.git>
    cd Quick-Reshponse-System
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Environment Variables:**
    Create a `.env` file in the root directory and add your Firebase configuration:
    ```env
    EXPO_PUBLIC_FIREBASE_API_KEY=your_api_key
    EXPO_PUBLIC_FIREBASE_AUTH_DOMAIN=your_auth_domain
    EXPO_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
    EXPO_PUBLIC_FIREBASE_STORAGE_BUCKET=your_storage_bucket
    EXPO_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_messaging_sender_id
    EXPO_PUBLIC_FIREBASE_APP_ID=your_app_id
    EXPO_PUBLIC_FIREBASE_MEASUREMENT_ID=your_measurement_id
    ```

4.  **Run the application:**
    ```bash
    npx expo start
    ```

    *   Press `a` to open on an Android emulator.
    *   Press `i` to open on an iOS simulator.
    *   Press `w` to open in the web browser.
    *   Scan the QR code with the **Expo Go** app on your physical device.

## 📱 Screens Overview

*   **SplashScreen:** Initial app loading and authentication check.
*   **Login/Signup:** Firebase-powered user authentication.
*   **HomeScreen:** Main dashboard with the primary SOS button.
*   **ContactsScreen:** Manage your trusted emergency contacts.
*   **MapScreen:** View your current location and nearby emergency services (custom implementations for web and native).
*   **AlertsScreen:** History and status of triggered alerts.
*   **ProfileScreen:** User details and settings.

