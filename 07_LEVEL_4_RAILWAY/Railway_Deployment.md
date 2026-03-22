# 🚂 Deploying Your App to Railway

When your project graduates from a simple React site to a Full-Stack application (maybe you had Antigravity build a custom Node.js Express server), you deploy it to Railway.

Here is the exact checklist for getting your complex application live on the web.

---

## ✅ Pre-Flight Checks

- [ ] Your code is fully pushed to the `main` branch on GitHub.
- [ ] Your app runs perfectly on your local machine.
- [ ] You have kept any secret keys (like API keys) OUT of your public code files!

---

## Step 1: Connect to Railway

1. Go to [railway.app](https://railway.app/).
2. Click **Login** and select **GitHub**. (Always authenticate with GitHub so platforms can access your repositories securely).
3. Once logged in to the dashboard, click the **New Project** button.
4. Select **"Deploy from GitHub repo"**.
5. Give Railway permission to see your repositories, and select your project from the list.

*Railway will immediately read your code, detect what kind of application it is, and start building it. However, it will likely fail on the first try if you need Database connections! Let's fix that.*

---

## Step 2: Adding a Database (If Needed)

If Antigravity built you an app that relies on a PostgreSQL or MySQL database, you need to spin one up on Railway.

1. On your Railway Project Canvas (the cool graph view showing your app), right-click anywhere in the empty space.
2. Select **"New Service"** -> **"Database"** -> **"Add PostgreSQL"** (or MySQL, depending on your app).
3. Wait 10 seconds. Railway has just built a complete, secure database for you.

## Step 3: Wiring it Together (Environment Variables)

Your Application container needs to know how to connect to the Database container you just built.

1. Click on your **PostgreSQL Database** box on the canvas.
2. Click the **"Connect"** tab. You will see a `DATABASE_URL` (it looks like a long string of random characters).
3. Now, click on your **Web Application** box on the canvas.
4. Click the **"Variables"** tab.
5. Add a "New Variable". 
   - Variable Name: `DATABASE_URL` (or whatever variable your code is expecting).
   - Value: Click the magic wand icon and choose the Database URL from the PostgreSQL service.
6. Does your app need other secrets? (e.g., an OpenAI key, an email password). Add them all here in the **Variables** tab so they are hidden and secure.

---

## Step 4: Generate a Public Domain

By default, Railway apps are completely private. We need to give it a public web address so people can visit it.

1. Click on your **Web Application** box on the canvas.
2. Click the **"Settings"** tab.
3. Scroll down to the **"Networking"** section.
4. Click **"Generate Domain"**.

Railway will give you a neat `.up.railway.app` URL. 

The moment you add a Variable or generate a Domain, Railway automatically kicks off a new Build. Wait about 60 seconds, watch the logs turn green, and then click your new link.

**You have just deployed Enterprise-Grade infrastructure using AI and Railway!**
