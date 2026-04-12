# 📝 The Master Prompt: Personal Bio Site

This is a **Master Prompt**. Think of it as a highly detailed script for our crew. We do not ask the AI to "make a website;" we tell it *exactly* what frameworks to use, what the vibe should be, and what content to include.

By using constraints, we guarantee a professional result. 

### Instructions:
1. Copy the text in the code block below.
2. Paste it into a new document on your computer (like Notepad or Word).
3. **Change the text in bracketed brackets** `[LIKE THIS]` to your personal information.
4. Copy your customized prompt and paste it into Google AI Studio.

---

<AIStudioLauncher 
  instructions="Copy this prompt, modify the bracketed information [LIKE THIS] to match your personal details, and paste it into Google AI Studio."
  prompt={`Act as an expert Frontend Developer and UI/UX Designer.

I need you to build a single-page Personal & Ministry Bio website.
This must be a completely contained artifact that I can easily deploy.

TECHNICAL CONSTRAINTS:
- Use React and Tailwind CSS.
- Provide all the code in a single, complete block (do not skip any code).
- Use Lucide React icons for the interface.
- Ensure the application is responsive on mobile and desktop.
- The design must be modern, clean, and professional.

AESTHETIC VIBE:
- Look and Feel: Clean, airy, peaceful, and solid. 
- Colors: Soft slate grays, muted sage greens, and clean white backgrounds. Use subtle gradients if necessary. Avoid harsh, bright colors.
- Typography: Use standard, modern sans-serif fonts (like Inter or Roboto). Ensure strong contrast for readability.
- Animations: Add simple hover states for buttons/links. Avoid complex animations that distract from the message.

CONTENT & STRUCTURE:
Please include the following sections on the page:

1. Hero Section (Top):
   - A welcoming headline: "Hi, I'm [YOUR NAME]."
   - A short, one-sentence subtitle: "[Example: Worship Leader, Teacher, and Community Builder.]"
   - A primary button: "Contact Me" (Links to the contact section).

2. About Me:
   - A clean paragraph introducing who you are, what ministry or field you serve in, and what drives you. Keep it to 3-4 sentences.
   - Example text (replace): "[I am deeply passionate about connecting people with purpose. For the last 10 years, I have worked with local communities to build bridges...]"

3. My Focus Areas (Cards):
   - Create 3 simple, beautifully designed cards.
   - Card 1: "[Youth Ministry] - [Short description]"
   - Card 2: "[Community Outreach] - [Short description]"
   - Card 3: "[Digital Discipleship] - [Short description]"
   - Give each card an appropriate Lucide icon.

4. Contact / Connect:
   - A simple list of ways to connect.
   - Email: "[your.email@example.com]"
   - Church/Organization Website: "[www.yourchurch.org]"
   - A concluding encouraging thought: "Let's build something good together."

Please write the full React component now.`} 
/>
