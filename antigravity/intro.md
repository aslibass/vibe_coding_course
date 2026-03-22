# 🚀 Level 2: The Agentic Era (Enter Antigravity)

Congratulations on graduating from the core Vibe Coding course! 

Up until now, you have been functioning as a **Director**. You wrote the script (the prompt), you handed it to the crew (AI Studio), they handed you back the footage (the code), and you manually spliced it together in your editing room (your code editor).

If you are ready to build faster, handle more complex projects, and let the AI do the manual labor of saving files and running terminal commands, it is time to become a **Manager**.

Welcome to Level 2. Welcome to **Antigravity**.

---

## 📅 The Post-Graduation Path

| Module | Description |
|---|---|
| **[Antigravity_Setup.md](./Antigravity_Setup.md)** | Learn how to install and interact with Antigravity, your new autonomous coding agent. |
| **[Agentic_Workflow.md](./Agentic_Workflow.md)** | The "Spec-and-Review" loop. How to hand off entire features (like a database integration) to Antigravity and review its pull requests. |
| **[Starter_Template_Prompt.md](./Starter_Template_Prompt.md)** | The master prompt to have Antigravity run terminal commands and build a React/Tailwind base from scratch. |

---

## 🤖 Core Concept: The Manager Mindset

When we used Google AI Studio, the AI was "trapped" in a chat box. It couldn't see your files unless you copied and pasted them. It couldn't run your application to see if it worked.

**Antigravity is an Agent.** 

An Agent is an AI that has hands and eyes. When you chat with Antigravity, it can:
1. **Read** every file in your project folder automatically without you pasting it.
2. **Write** changes directly to your code files.
3. **Run** terminal commands (like starting your server or deploying your code).
4. **See** the results of those commands and fix its own errors before it even tells you about them!

<BlueprintDiagram mermaidCode={`graph TD;
  User[You] -->|Spec| Agent[Antigravity];
  Agent -->|Reads Files| IDE[Code Editor];
  Agent -->|Writes Code| IDE;
  Agent -->|Runs Commands| Terminal;
  Terminal -->|Logs/Errors| Agent;`}/>

As a Manager, your job shifts from manually moving code around to simply providing excellent **Spec Sheets** and reviewing the work Antigravity does on your behalf.

You still need the **Precision of Intent** you learned in Session 1, but now the machine takes care of the copy/pasting.

Let's learn how to manage an Agent!


---

## 📺 Curated Required Viewing
- **[What are AI Agents? (IBM Technology)](https://www.youtube.com/watch?v=F8NKVhkZZWI)**: A perfect visualization of the difference between a chatbot and an autonomous Agent.
- **[Andrew Ng: Agentic Reasoning](https://www.youtube.com/watch?v=sal78ACtGTc)**: A mandatory watch on how agentic workflows (reflection, tool use) outperform standard AI prompting.
