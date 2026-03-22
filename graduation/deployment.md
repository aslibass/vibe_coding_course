# 🚀 Deployment Checklist

Your application works on your computer. Your database is secure. You have a login system.

Now, we put it on the public internet so you can text the link to your friends, family, and church members.

We will use a free, incredibly powerful service called [Vercel](https://vercel.com/) (or optionally Netlify) to host our Vite/React application. This usually takes less than 5 minutes!

---

## ✅ Pre-Flight Checks

Before we deploy, double-check your local application:

- [ ] I can successfully log in and log out using the Google button.
- [ ] I can submit a Praise report, and it appears in the feed immediately.
- [ ] If I refresh the page, the Praise reports remain (data is persisting to Firebase).
- [ ] My code is cleanly formatted and saved in my code editor.

---

## 📦 Step 1: Push Your Code to GitHub

Vercel (our host) doesn't take code directly from your computer. Instead, it "watches" your GitHub account. When you put new code in GitHub, Vercel automatically grabs it and deploys it.

1. Open your terminal/command prompt in your project folder.
2. If you haven't recently, commit and push your changes:
   ```bash
   git add .
   git commit -m "Final version ready for deployment"
   git push origin main
   ```
3. Go to `github.com` in your browser and verify that your newest code is sitting in your repository.

---

## 🌍 Step 2: Connect to Vercel

1. Go to [vercel.com](https://vercel.com/).
2. Click **Sign Up** (or Log In).
3. Choose the option to **"Continue with GitHub"**. This links Vercel directly to your "digital public library."
4. Once you are logged into the Vercel dashboard, click the black **"Add New..."** button and select **Project**.
5. You will see a list of your GitHub repositories. Find the one containing your Miracle Tracker app (e.g., `miracle-tracker-app`) and click **Import**.

---

## ⚙️ Step 3: Configure the Build

Vercel is very smart. It usually detects that you are using React and Vite and sets things up automatically. But we need to check one thing.

1. **Project Name:** You can leave it as default or change it depending on what you want the URL to be.
2. **Framework Preset:** Vercel should auto-detect and show **"Vite"**. If it doesn't, click the dropdown and select it.
3. **Environment Variables:** If you hard-coded your Firebase keys into your React file, you can skip this for now (since we aren't handling highly sensitive enterprise data yet). *Note: In a professional setting, we would hide the keys here!*
4. Click the large **Deploy** button.

---

## 🎉 Step 4: Watch the Confetti

The screen will change. Vercel is now downloading your code, building the production version of the application, and uploading it to servers around the world.

This takes about 30 to 60 seconds.

When it finishes, the screen will shower you with digital confetti! 🎊 

Click on the screenshot of your application to go to your live URL (e.g., `https://miracle-tracker-xyz.vercel.app`).

**Test it immediately:** Log in on the live site, post a praise, and make sure it works. 

**Congratulations. You are officially a Vibe Coder. Text that link to the group chat!**
