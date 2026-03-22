# 🏗️ The Antigravity Starter Prompt (Scaffolding)

If you are starting a brand new project and do not want to copy/paste the `starter-template` folder provided in this repository, you can have Antigravity build the entire environment for you!

Unlike Google AI Studio (which just gives you code to copy), **Antigravity can run your terminal and write your files.**

Just open a new, blank folder in your code editor, open Antigravity, and paste the exact prompt below. Antigravity will do all the heavy lifting in about 30 seconds.

---

### Copy and Paste this into Antigravity:

```text
Act as an expert Frontend Developer and build a local sandbox for me.

Please execute the terminal commands to scaffold a new React project in this current directory using Vite (use the `react` template). Do not put it in a sub-folder; initialize it right here.

Once the scaffolding is complete, please run the following installations:
1. Install standard dependencies (`npm install`).
2. Install Tailwind CSS and its peers (`npm install -D tailwindcss postcss autoprefixer`).
3. Install our primary libraries (`npm install lucide-react firebase`).

After installation:
1. Initialize `tailwind.config.js` and configure it to scan the `./index.html` and `./src` paths for content.
2. Initialize `postcss.config.js`.
3. Wipe out the default CSS in `src/index.css` and replace it entirely with the three core `@tailwind` directives.
4. Replace `src/App.jsx` with a clean, centered, well-styled placeholder screen that says "Welcome to the Vibe Coding Sandbox" using Tailwind classes (slate, white, and a slight shadow). 

When you are completely finished, let me know, but do not start the dev server yourself. I will start it when I am ready.
```

---

### What Happens Next?
1. You will see Antigravity start furiously executing commands in the background.
2. It will write the config files.
3. When it says it is done, simply type `npm run dev` in your terminal and click the `localhost` link to see your brand new, perfectly configured Sandbox!
