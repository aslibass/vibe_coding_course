# 🧗 Micro-Vibe Challenges

It is time to practice iteration and the T-A-O loop! We will modify the Bio Sites we created in Session 1.

You are going to ask the AI to add new features to your existing, working code. It is highly recommended to practice the screenshot technique we learned in the `Debugging_Guide.md`.

Try to complete these three challenges.

---

## 🕒 Challenge 1: The Event Countdown Timer

**The Goal:** Add a dynamic timer counting down to a specific upcoming event on your Bio Site.

**The Prompt Framework:**
1. Copy all the current, working code of your Bio site.
2. Paste it into a fresh Google AI Studio chat (or continue in the old one) and say:
   <AIStudioLauncher prompt={`Here is my current code snippet: `[PASTE CODE]`. I want you to modify this by adding a new section right below the Hero Section. This new section should contain a live Countdown Timer for an event called 'City Outreach Team Meeting'. Set the date for this Friday at 6:00 PM. Make sure the countdown visually updates every second. Use a dark background to make this timer section pop out from the rest of the site.`} instructions="Use this prompt structure in AI Studio to add a countdown timer." />

**The Observation:** Did it place the timer in the right spot? Does it tick down? 

---

## 🌗 Challenge 2: The Dark Mode Toggle

**The Goal:** Add a button that lets the user switch between a light aesthetic and a dark aesthetic.

**The Prompt Framework:**
1. Make sure you are using your newest code (with the timer included!).
2. Give the AI this challenge:
   <AIStudioLauncher prompt={`We need to add a Dark Mode to this application. Please create a small toggle button (use a Sun icon for light mode, and a Moon icon for dark mode from Lucide React). Place this button fixed in the top right corner of the screen. When the user clicks the button, the entire application's color scheme should invert to a modern, sleek dark mode. Ensure all text remains highly readable.`} instructions="Use this prompt to add a dark mode toggle." />

**The Observation:** Does the button exist? Does the color scheme change? Did it break the colors of your buttons or headers? If it looks ugly in dark mode, take a screenshot and ask the AI to fix specific color clashing!

---

## 📨 Challenge 3: A Pop-up Contact Form

**The Goal:** Change the simple "Contact" list at the bottom of the page into a button that opens a professional modal (pop-up) form.

**The Prompt Framework:**
   <AIStudioLauncher prompt={`Currently, my contact info is just listed at the bottom of the page. Replace this section entirely. I want a large, centered button that says 'Send a Message'. When clicked, it should open a beautiful modal (pop-up) in the center of the screen with a blurred background behind it. The form inside the modal should ask for Name, Email, and Message, and have a 'Submit' and 'Cancel' button. For now, the submit button doesn't need to do anything, just close the modal. Make sure the modal matches the aesthetic of the site (dark or light depending on the toggle!).`} instructions="Use this prompt to create a pop-up contact form modal." />

**The Observation:** Does the screen blur behind it? 

---

If you can complete all three of these challenges, you have successfully mastered the art of iterative prompting!
