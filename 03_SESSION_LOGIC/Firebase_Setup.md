# 🔑 Firebase Setup Guide 

Firebase is our Filing Cabinet. It's incredibly powerful but intimidating at first glance. Don't worry! We only need to do exactly these steps to get our keys.

---

## Phase 1: Create the Project

1. Go to [console.firebase.google.com](https://console.firebase.google.com/). Ensure you are logged in with the Google Account you created in Week 0.
2. Click the big **"Add Project"** (or Create Project) button.
3. Enter a name: `Miracle-Tracker` (or whatever you prefer). Click Continue.
4. **Google Analytics:** You will be asked if you want to enable Google Analytics. **Turn this OFF.** (Toggle the switch to the left). Click Create Project.
5. Wait for the loading circle. When it's done, click **Continue**.

---

## Phase 2: Create the Filing Cabinet (Firestore)

Your project is created, but we need to specifically turn on the Database feature.

1. On the left-hand menu, click on **Build**, then click on **Firestore Database**.
2. Click the **"Create Database"** button.
3. **Location:** Leave the location as the default (usually `nam5` or `us-central`). Click Next.
4. **Security Rules:** Select **"Start in Test Mode"**. 
   - *(Note: This allows anyone to read/write data for 30 days. It is perfect for learning. In Week 4, we will learn how to lock this down!)*
5. Click **Enable**.
6. Wait a few seconds. You should now see an empty "Data" panel staring back at you. Your database is ready!

---

## Phase 3: Get Your Keys (Web App Config)

Our React code needs a specific set of keys to know which database to talk to.

1. In the left-hand menu, click the **Gear Icon** (Project Settings) next to the "Project Overview" button at the top left.
2. Scroll down to the bottom where it says **"Your apps"**.
3. Click the icon that looks like this: `</>` (This represents a Web App).
4. Enter an App nickname (e.g., `Tracker Web App`). 
5. Skip "Also set up Firebase Hosting". Click **"Register app"**.
6. A box will appear with code inside it. You are looking for a section that looks exactly like this:

```javascript
const firebaseConfig = {
  apiKey: "AIzaSyB-xxxxxxxxxxxxxxx",
  authDomain: "miracle-tracker-xxx.firebaseapp.com",
  projectId: "miracle-tracker-xxx",
  storageBucket: "miracle-tracker-xxx.firebasestorage.app",
  messagingSenderId: "1234567890",
  appId: "1:1234567890:web:abcdefg12345"
};
```

7. **COPY EVERYTHING from the word `const` down to the `};`**. 
8. Keep this safe! When you generate the code using your `Miracle_Tracker_Spec.md`, you will paste these exact keys into the designated spot in your new React code.

You now own a working, cloud-hosted database!
