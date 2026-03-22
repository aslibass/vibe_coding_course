# 🔄 The Agentic Workflow: Spec-and-Review

When you are using an Agent like Antigravity, the T-A-O Loop (Thought -> Action -> Observation) evolves. You will spend much less time copy/pasting code, and much more time writing excellent Specifications and reviewing the Agent's work.

This is the **Spec-and-Review** workflow.

---

## Phase 1: Planning (The Spec)

Just like the `Miracle_Tracker_Spec.md` we used in Session 3, you should write down exactly what you want the Agent to build *before* you prompt it.

Because Antigravity can read files, the best way to do this is to create a temporary Markdown file right inside your project folder!

1. Create a file called `todo.md` (or `plan.md`) in your project.
2. Write down your requirements clearly.
   - Example: *"We need a new page for 'Team Bios'. It needs a grid of 6 cards showing a photo, name, and fun fact. The photos should be circular."*

---

## Phase 2: Handoff (The Prompt)

Instead of pasting a massive prompt into the chat, you simply point Antigravity to the file you just made.

**Your prompt is now just one sentence:**
> "Please review `todo.md` and implement the 'Team Bios' page as described. Let me know when you are finished."

Antigravity will:
1. Open and read `todo.md`.
2. Create the new React component file.
3. Hook up the routing so the page is accessible.
4. Modify your navigation bar to include a link to the new page.

---

## Phase 3: Review & Course Correction

**CRITICAL: Treat Antigravity like a Junior Developer on your team.** It is fast, but it can hallucinate or make mistakes. You must review its work before assuming it is complete.

1. Open your code editor and use the Source Control (Git) tab to review exactly which lines of code Antigravity modified.
2. Open your application in the browser.
3. Click on the new "Team Bios" link and test the functionality.
4. Observe the result. 

If it's perfect, merge the changes and celebrate!
If it's slightly wrong (e.g., the photos are squares instead of circles), you simply reply to Antigravity:
> "The page looks great, but the photos are currently squares. In the `todo.md` spec, I requested circular photos. Please update the CSS to make them circular."

Antigravity will use its tools, locate the specific CSS file, fix the corners, and report back.

---

## 🎓 The Paradigm Shift

**Vibe Coding Level 1:** You are the typist. The AI tells you what to type.
**Vibe Coding Level 2:** You are the manager. You point at a problem, the AI types the code, and you approve it.

By mastering the Spec-and-Review workflow, you can build applications of incredible complexity. You can tell Antigravity, *"Read the documentation for this new Payment Gateway and build a checkout screen for our church retreat."*

The machine works for you now!
