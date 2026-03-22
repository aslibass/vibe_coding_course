# 🛡️ Authentication & Security Guide

We need to add a "Bouncer" to our application so we know who is posting Praises. We will do this by telling the AI to add a "Sign in with Google" button.

Once they sign in, we need to lock the Filing Cabinet (Firebase) so only signed-in people can add new Praises.

---

## 🚪 Step 1: Prompting for the Google Login Button

We will ask Google AI Studio to modify our existing Miracle Tracker. 

**The Prompt Framework:**
1. Copy your latest, working code for the Miracle Tracker.
2. Paste it into Google AI Studio and say:
   > "Here is my current code: `[PASTE CODE]`. I need you to add Google Authentication to this. 
   > 
   > 1. Add a 'Sign in with Google' button to the header instead of the 'Share a Praise' button if the user is not logged in.
   > 2. Once they are logged in, show their profile picture (small) and a 'Sign Out' button in the header. Only show the 'Share a Praise' button if they are signed in.
   > 3. When they submit a Praise, automatically use their Google display name as the 'author' instead of letting them type it in, and save their `uid` (user ID) to the document.
   > 
   > Please provide the updated React component."

3. Test the new code. The button won't completely work yet because we have to flip a switch in Firebase first!

---

## 🔑 Step 2: Enabling Google Sign-In in Firebase

Your application is asking Firebase to log a user in, but Firebase doesn't know it's allowed to do that yet.

1. Go back to your Firebase Console (`console.firebase.google.com`).
2. Click on your `Miracle-Tracker` project.
3. On the left menu, click **Build**, then click **Authentication**.
4. Click the **"Get Started"** button.
5. You will see a list of "Sign-in providers." Click on **Google**.
6. Switch the **Enable** toggle to ON (Blue).
7. Under "Project support email," click the dropdown and select your email address.
8. Click **Save**.

Now, go back to your local app running on your computer and try clicking the "Sign in with Google" button. A pop-up should appear, and you should be able to log in!

---

## 🧱 Step 3: Locking the Filing Cabinet (Security Rules)

Currently, our database is in "Test Mode"—meaning anyone with our keys can delete all our testimonies. We need to add rules.

1. In the Firebase Console, on the left menu, click **Firestore Database**.
2. Near the top middle of the page, click the tab that says **"Rules"**.
3. You will see code that looks something like this:
   ```javascript
   rules_version = '2';
   service cloud.firestore {
     match /databases/{database}/documents {
       match /{document=**} {
         allow read, write: if request.time < timestamp.date(2025, 12, 31);
       }
     }
   }
   ```
4. **Delete everything** in that box.
5. Paste in our secure configuration:
   ```javascript
   rules_version = '2';
   service cloud.firestore {
     match /databases/{database}/documents {
       
       // Rules for the 'praises' collection
       match /praises/{praiseId} {
         // ANYONE can read the praises (public feed)
         allow read: if true;
         
         // ONLY SIGNED-IN users can create a new praise
         allow create: if request.auth != null && request.auth.uid == request.resource.data.uid;
         
         // ONLY the user who created it can delete or modify it
         allow update, delete: if request.auth != null && request.auth.uid == resource.data.uid;
       }
     }
   }
   ```
6. Click the beautiful blue **Publish** button.

Congratulations! Your database is now secure. Only verified people can post, and no one can tamper with the data. You are ready to deploy.
