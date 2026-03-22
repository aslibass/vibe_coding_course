# 💻 Local Environment Setup

In order to actually *see* the code that AI Studio gives you, you need a place to put it and run it on your own computer. This is called your "Local Environment."

Follow these instructions exactly!

---

## 1. Install Node.js (The Engine)
Modern web development runs on a background engine called Node.js. 
1. Go to [nodejs.org](https://nodejs.org/).
2. Download the version that says **"LTS"** (Long Term Support).
3. Run the installer and just click "Next" / "Agree" through the default settings.

## 2. Install VS Code (The Editor)
You cannot easily paste code into Microsoft Word. We need a specialized text editor.
1. Go to [code.visualstudio.com](https://code.visualstudio.com/).
2. Download and install **Visual Studio Code**.
*(Alternatively, you can download **Cursor**, which is an AI-powered version of VS Code if your group prefers a native AI editor).*

## 3. Meet Your Terminal (The Command Room)
Inside VS Code, you can open a "Terminal." This is a black box where you type special commands to turn your application on and off.
1. Open Visual Studio Code.
2. At the very top menu, click `Terminal` -> `New Terminal`. A panel will appear at the bottom.

If you are on **Windows**, this will default to **PowerShell**.
If you are on **Mac**, this will default to **Zsh/Bash**.

### ⌨️ The 3 Magic Terminal Commands You Need to Know:
Whenever you download the `starter-template` or a new project from a teammate, open it in VS Code, open the Terminal, and type these (press Enter after each):

1. `npm install`
   *(This tells Node.js to download all the necessary background files. You only need to do this ONCE per project.)*
2. `npm run dev`
   *(This actually starts your website on your local machine! It will give you a link like `http://localhost:5173`. Click that link to view your app!)*
3. **To turn it off:** Click inside the terminal box and press `Ctrl + C` on your keyboard. 

---

## 4. Setting up Antigravity (Level 2 Preparation)
While we will mostly use Google AI Studio for Weeks 1 through 4, setting up **Antigravity** (your autonomous coding Agent) now is highly recommended. 

When you configure Antigravity inside your code editor, it gains the ability to:
- Run `npm run dev` for you automatically.
- Paste the code into your files without you lifting a finger.
- Tell you exactly what errors are happening internally.

Make sure you've installed the Antigravity extension/interface in your IDE (Cursor or VS Code integration) during this Pre-Flight stage, and ensure you are logged into your AI platform. When you reach the Level 2 modules, you will rely entirely on this Agent!
