# 📋 App Spec: The Miracle Tracker (Praise Report App)

For more complex applications that have data (like databases), a single prompt sometimes isn't enough. We need to give the AI a **Specification Sheet** (a Spec). 

Think of a Spec like a blueprint for a house. It tells the builder exactly how many rooms there are and what goes in them.

We are going to give this entire document to Google AI Studio.

---

### Copy everything below this line and paste into Google AI Studio:

```text
Act as a Senior Full-Stack Engineer.

I need you to build a single-page Web Application called the "Miracle Tracker" (A Praise Report App). 

This application must allow users to submit short testimonies/praises, save them to a Firebase Firestore database, and display a feed of all submitted praises in real-time.

TECHNICAL CONSTRAINTS:
- Use React and Tailwind CSS.
- Use Lucide React for all iconography.
- Use Firebase version 10+ (modular syntax).
- Please provide the complete Code block. DO NOT use any placeholders for the main logic. You must handle the complete Firebase initialization and export the `db` instance. I will only paste my `firebaseConfig` block; you must do the rest.
- Provide instructions on how to install necessary dependencies (e.g., firebase).

AESTHETIC VIBE:
- Vibe: Joyful, clean, warm, and highly readable.
- Colors: White backgrounds, warm yellow/gold accents for buttons or highlights, soft gray text for readability.
- Layout: Mobile-first design focusing on a single, scrolling column.

DATA STRUCTURE (FIRESTORE):
We need a single collection called `praises`.
Each document in `praises` should contain:
- `title` (string): A short headline for the testimony.
- `story` (string): The detailed description of what happened.
- `author` (string): Name of the person sharing (or "Anonymous").
- `category` (string): A dropdown selection (Healing, Provision, Breakthrough, Protection, Other).
- `createdAt` (timestamp): The date it was submitted for sorting.
- `celebrationCount` (number): Simple counter for a "Like/Amen" button.

APPLICATION FEATURES:

1. Header:
   - App title: "The Miracle Tracker" with a spark or star icon.
   - A button: "Share a Praise" (Opens a modal to submit a new story).

2. The Feed (Main Content):
   - Display a list of all items from the `praises` collection, sorted by newest first.
   - Each praise should look like a card.
   - The card should show the Category as a small badge (styled differently depending on the category).
   - The card should show Title, Story, Author, and Date.
   - Include a button on each card: "Praise God! (Count)" referencing the `celebrationCount`. Clicking this increments the count in Firebase.

3. "Share a Praise" Modal (Form):
   - A clean pop-up form with fields mapping exactly to the Data Structure.
   - Text input for Title.
   - Textarea for Story.
   - Text input for Author.
   - Dropdown (select) for Category.
   - Submit Button: "Post Testimony". Disabled while submitting to prevent double posts. Show a loading spinner if possible.

CORE REQUIREMENT:
Write the complete React component. Please include a standard Firebase configuration block at the top of the file that I can easily replace with my own `firebaseConfig` object. Assume we are not using user authentication for this version—anyone can read, write, and click the celebrate button.
```
