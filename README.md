![Banner](https://github.com/thanhbinh-ic/AI-Roleplay-Simulator/blob/6cae6fed33fdb13490df0b8c2c2f1212f505c1fd/docs/img/Banner.webp)

# 🚀 AI Roleplay Simulator (AI-Powered RPG)

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-039BE5?style=for-the-badge&logo=Firebase&logoColor=white)
![Gemini AI](https://img.shields.io/badge/Gemini_AI-4285F4?style=for-the-badge&logo=google-gemini&logoColor=white)

**AI Roleplay Simulator** is an interactive text adventure game where Artificial Intelligence acts as your personal "Dungeon Master." The system dynamically generates worlds, characters, and branching storylines based on your unique creative inputs, offering a limitless storytelling experience.

---

## 📥 Get Started Now

Experience the simulator instantly or download the latest standalone version:

[![Gemini Canvas](https://img.shields.io/badge/LIVE_DEMO-GEMINI_CANVAS-blue?style=for-the-badge&logo=google-gemini&logoColor=white)](https://gemini.google.com/share/f772733ac3af) 
[![Vercel App](https://img.shields.io/badge/LIVE_DEMO-VERCEL_APP-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://ai-roleplay-simulator.vercel.app/)
[![Download Latest Version](https://img.shields.io/badge/DOWNLOAD-LATEST_RELEASE-success?style=for-the-badge&logo=github)](https://github.com/thanhbinh-ic/AI-Roleplay-Simulator/releases/latest)

> [!IMPORTANT]
> **API Key Requirement:** If you are deploying or using the **Vercel version**, please ensure you have configured a valid `REACT_APP_GEMINI_API_KEY`. Using the default or shared keys may lead to **Quota Limit Errors** due to high traffic.

---

## ✨ Key Features

### 🧠 Intelligent AI Dungeon Master
- **Dynamic World Building:** AI automatically suggests Character Names, Starting Skills, Goals, and Backstories based on your chosen setting.
- **Narrative Continuity:** Advanced memory management ensures the AI follows story logic, character traits, and past events.

### 🎲 Advanced Gameplay Mechanics
- **Diverse Difficulty Levels:** From casual storytelling to "Nightmare" mode where every choice could be your last.
- **Adult Content Support (18+):** Allows for extremely detailed, mature, and uncensored narratives for a truly unrestricted roleplaying experience.
- **Dice System:** A transparent rolling mechanism with 5 success tiers, calculated based on character stats and current status.
- **Quest System:** Real-time AI quest generation with a dedicated "Quest Log" to track objectives and rewards.

### 💾 Data & System Management
- **Cloud & Local Saving:** Support for Firebase Firestore syncing or local `.json` file exports for cross-platform play.
- **Auto-Update System:** Seamlessly checks for new versions via GitHub Gist to ensure you always have the latest fixes and features.

---

## 🛠 Tech Stack

- **Frontend:** React.js & Tailwind CSS (Modern, responsive UI).
- **Backend/Database:** Firebase Firestore & Authentication.
- **AI Engine:** Google Gemini API (or compatible Large Language Models).
- **Version Control:** GitHub Gist API for the automated Update System.

---

## 📸 Screenshots

| Main Menu | Gameplay Interface |
| :---: | :---: |
| ![Start](https://github.com/thanhbinh-ic/AI-Roleplay-Simulator/blob/6cae6fed33fdb13490df0b8c2c2f1212f505c1fd/docs/img/Main-Menu.webp) | ![Gameplay](https://github.com/thanhbinh-ic/AI-Roleplay-Simulator/blob/6cae6fed33fdb13490df0b8c2c2f1212f505c1fd/docs/img/Gameplay-Interface.webp) |

---

## 📜 Changelog

### v2.5 (Experience & Connectivity) - 2026-04-07
- **CRITICAL:** Fixed application crash (Initialization Error) during startup version check.
- **NEW:** Added manual "Check for Updates" button on the main menu.
- **UPDATE:** Implemented Static Redirect mechanism for more reliable download links.
- **UI:** Enhanced Update Modal with Backdrop Blur and smooth entrance animations.
- **STABILITY:** Integrated Cache-Busting parameters to ensure instant synchronization with Gist updates.

---

<h2>🚀 Installation & Deployment (For Developers)</h2>

<p align="center">
  <i>This guide provides a "hand-holding" walkthrough to deploy your own instance of the Simulator.</i>
</p>

<blockquote>
  <strong>Note:</strong> While this project can be deployed on various platforms, this documentation focuses on <strong>Vercel.com</strong> for its seamless integration with React and GitHub.
</blockquote>

<details>
  <summary><strong>1. Forking & Local Setup</strong></summary>
  <br />
  <ol>
    <li>Go to the <a href="https://github.com/thanhbinh-ic/AI-Roleplay-Simulator">Original Repository</a>.</li>
    <li>Click the <strong>Fork</strong> button in the top-right corner to create a copy under your account.</li>
    <li>Clone your fork to your machine:
      <pre><code>git clone https://github.com/your-username/AI-Roleplay-Simulator.git
cd AI-Roleplay-Simulator</code></pre>
    </li>
    <li>Install the necessary packages:
      <pre><code>npm install</code></pre>
    </li>
  </ol>
</details>

<details>
  <summary><strong>2. Firebase Configuration (Database & Auth)</strong></summary>
  <br />
  <ol>
    <li>Go to the <a href="https://console.firebase.google.com/">Firebase Console</a> and click <strong>Add Project</strong>.</li>
    <li><strong>Authentication:</strong> 
      <ul>
        <li>Navigate to <i>Build > Authentication</i> and click <strong>Get Started</strong>.</li>
        <li>Enable <strong>Email/Password</strong> provider.</li>
      </ul>
    </li>
    <li><strong>Firestore Database:</strong>
      <ul>
        <li>Navigate to <i>Build > Firestore Database</i> and click <strong>Create database</strong>.</li>
        <li>Start in <strong>Test Mode</strong> (you can update rules later).</li>
      </ul>
    </li>
    <li><strong>Get Your Config:</strong>
      <ul>
        <li>In Project Settings, scroll to "Your apps" and add a <strong>Web App</strong>.</li>
        <li>Copy the <code>firebaseConfig</code> values. They will look like this:</li>
      </ul>
      <pre><code>const firebaseConfig = {
  apiKey: "AIzaSy...",
  authDomain: "...firebaseapp.com",
  projectId: "...",
  storageBucket: "...firebasestorage.app",
  messagingSenderId: "...",
  appId: "..."
};</code></pre>
    </li>
  </ol>
</details>

<details>
  <summary><strong>3. Gemini AI API Setup</strong></summary>
  <br />
  <ol>
    <li>Visit <a href="https://aistudio.google.com/">Google AI Studio</a>.</li>
    <li>Click <strong>Get API key</strong> in the sidebar.</li>
    <li>Select <strong>Create API key in new project</strong>.</li>
    <li><strong>Verify your Key:</strong> Paste this URL in your browser (replace <code>YOUR_KEY</code>) to see supported models:
      <br />
      <code>https://generativelanguage.googleapis.com/v1beta/models?key=YOUR_KEY</code>
    </li>
  </ol>
</details>

<details>
  <summary><strong>4. Deploying to Vercel</strong></summary>
  <br />
  <ol>
    <li>Create an account at <a href="https://vercel.com/">Vercel.com</a> using your GitHub.</li>
    <li>Click <strong>Add New > Project</strong> and import your forked repository.</li>
    <li><strong>Environment Variables:</strong> This is the <u>most important</u> step. Add these keys with your values:
      <ul>
        <li><code>REACT_APP_FIREBASE_API_KEY</code></li>
        <li><code>REACT_APP_FIREBASE_AUTH_DOMAIN</code></li>
        <li><code>REACT_APP_FIREBASE_PROJECT_ID</code></li>
        <li><code>REACT_APP_FIREBASE_STORAGE_BUCKET</code></li>
        <li><code>REACT_APP_FIREBASE_MESSAGING_SENDER_ID</code></li>
        <li><code>REACT_APP_FIREBASE_APP_ID</code></li>
        <li><code>REACT_APP_GEMINI_API_KEY</code></li>
      </ul>
    </li>
    <li>Click <strong>Deploy</strong>. Vercel will build your app and provide a live URL!</li>
  </ol>
</details>

<details>
  <summary><strong>5. Troubleshooting & Deployment Notes</strong></summary>
  <br />
  <ul>
    <li><strong>Routing Fix:</strong> If you get a 404 error when refreshing the page on Vercel, ensure you have a <code>vercel.json</code> in the root folder with a rewrite rule to <code>index.html</code>.</li>
    <li><strong>API Limits:</strong> If using the free tier of Gemini, be aware of the RPM (Requests Per Minute) limits.</li>
  </ul>
</details>

<hr />
  
---

## 🤝 Support & Contribution

- If you enjoy this project, **please give it a ⭐ Star!**.
- **Developer:** [thanhbinh-ic](https://github.com/thanhbinh-ic)

_Built with passion for RPG lovers and AI enthusiasts._
