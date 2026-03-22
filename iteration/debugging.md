# 🛠️ Debugging Guide: When the Machine Breaks

You wrote the perfect prompt. You pressed "Generate." Google AI Studio gave you the code. You pasted it, hit save, and... 

*RED SCREEN OF DEATH.* Or worse, it looks terrible.

This is not a failure. This is part of the process.

Here is how you handle issues gracefully. Don't panic. Direct the machine.

---

## Scenario A: Red Error Screens (Syntax & Logic Errors)

When the application refuses to run and shows a huge block of red or white error text, the AI made a mistake in the code.

**How to fix it:**
1. Do not try to read or understand the long error message (unless you want to).
2. Simply copy the **entire red error block**.
3. Go back to Google AI Studio.
4. Paste the error message directly into the chat and say: 
   > "I got this error when I tried to run the React application you just gave me. Please review and provide the fixed code."
5. The AI will generally recognize its mistake and give you a corrected version. Copy it, paste it over the old code, and try again.

---

## Scenario B: The Design looks Wrong (Layout & UI Issues)

Sometimes the app runs fine, but the button is overlapping the picture, the text is too small, or the colors clash.

The AI can't *see* the result like you can, so you have to be its eyes. The easiest way to fix Visual Issues is to use screenshots.

**How to fix it:**
1. Take a screenshot of the broken visual element. (On Windows: `Windows Key + Shift + S`. On Mac: `Command + Shift + 4`).
2. Go back to Google AI Studio.
3. Paste the screenshot directly into the chat.
4. Tell the AI exactly what is wrong in the image. Be precise.
   > "As you can see in the screenshot, the 'Contact Me' button is covering the bottom half of the image. It needs to be moved to the separate container below the image."
5. Review the new code it provides, paste it in, and check if it fixed the issue.

---

## Scenario C: The Blank White Screen

This is the scariest one because there is no obvious error. You open the app, and nothing is there. 

This usually means there is an error in the "Console" running in the background.

**How to fix it:**
1. Right-click anywhere on the blank white website screen.
2. Select **"Inspect"** from the menu. (A side panel will open).
3. In that side panel, look for the word **"Console"** at the top and click it.
4. Read through the text. You will almost certainly see red error text hiding in there.
5. Copy that red error text from the Console, paste it into Google AI Studio, and tell it:
   > "The page is rendering totally blank. Here is the error from the Chrome Developer Console. Please provide the fix."

---

Remember: The Director never panics when an actor misses a line. They simply give a clearer cue and retake the shot. The T-A-O loop is your friend.
