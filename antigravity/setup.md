# 🛠️ Antigravity Setup & Basics

Antigravity is your personal AI Software Engineer. Instead of chatting in a browser tab, Antigravity integrates directly into your coding environment (or runs locally on your machine), meaning it has access to your actual files.

---

## 1. What does it mean that Antigravity is an "Agent"?

A normal AI (like standard AI Studio) is a **Chatbot**. It answers questions.
An Agent is a system that can take **Actions**.

When you ask a Chatbot: *"Add a dark mode button."*
It responds: *"Here is the code to add a dark mode button. Please paste it into your `index.jsx` file."*

When you ask Antigravity: *"Add a dark mode button."*
It responds: *(Thinks)* -> *(Reads your `index.jsx` file)* -> *(Modifies the file directly)* -> *(Checks if it broke anything)* -> *"I have added the dark mode button to your header. You can view the changes now."*

---

## 2. Navigating the Antigravity Interface

When you interact with Antigravity, you will still type prompts just like you did in Week 1, but you will notice the AI starts displaying "Tool Calls".

**Common Tools Antigravity uses:**
- `view_file`: Antigravity is looking inside your Code to see how you built things.
- `write_to_file`: Antigravity is creating a brand new component or page.
- `multi_replace_file_content`: Antigravity is surgically editing exactly three lines of code in your file to fix a bug, leaving everything else untouched.
- `run_command`: Antigravity is using your terminal (e.g., to install Firebase for you).

*Do not be alarmed when you see it talking to itself or using tools! It is just working.*

---

## 3. The Power of "Context"

With AI Studio, if you started a new chat, the AI forgot who you were and what your app looked like.

With Antigravity, it can read your whole project. You can simply say:
> "I want to change the primary button color from blue to green."

You don't need to paste the button code! Antigravity will use its tools to search your files, find where the button is defined, and change it for you.

---

## 4. The Golden Rule of Agents: Trust but Verify

Because Antigravity can edit your files directly, it is incredibly fast. However, just like managing a junior developer on a human team, you must review their work.

Always use Git (or check your file history) to see what Antigravity changed before you deploy it to the public. If it made a mistake, you can just tell it:
> "That change broke the layout of the homepage. Please revert it and try moving the button to the footer instead."

Welcome to the future of software development!
