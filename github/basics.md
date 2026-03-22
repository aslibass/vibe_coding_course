# 📦 Version Control Basics

If you are going to let an Agent code for you, you need to save your work often.

We use **Git** (the software on your computer) and **GitHub** (the website where Git sends the data) to accomplish this.

Here are the three fundamental commands you need to memorize. Think of this as the "Save, Package, and Ship" routine.

---

## 1. `git add .` (The Shopping Cart)

Before you buy things at the store, you put them in your shopping cart. 
When you make changes to your code (or when Antigravity makes changes), Git notices them, but it doesn't save them permanently yet.

By typing `git add .` in your terminal (the `.` means "everything"), you are putting all changed files into your digital shopping cart, getting them ready to be properly saved.

## 2. `git commit -m "Your Message"` (The Receipt)

Now that your files are in the cart, you check out. 
A **Commit** is the actual, permanent snapshot in time. The message `-m "Added the dark mode button"` is the receipt. It tells Future You exactly what changed in this exact snapshot.

**Examples of good commit messages:**
- `git commit -m "Fixed the overlap bug on the hero image"`
- `git commit -m "Antigravity setup the Firebase database config"`

*Rule of Thumb: Commit your code every time you get a feature working perfectly. Never commit broken code.*

## 3. `git push origin main` (Shipping it to the Library)

Your commits (`add` and `commit`) only exist on your local laptop. If you spill coffee on your laptop right now, the code is gone.

**Push** takes all those safe snapshots you just made and securely uploads them to the GitHub cloud.

---

## 🛟 The Panic Button (How to Time Travel)

What happens if Antigravity completely breaks your app, and you want to go back to your last successful `commit`?

*Warning: This will delete any unsaved changes you have made since your last commit.*

If you want to throw away all the broken changes and reset to your last clean snapshot, simply type:

```bash
git restore .
```

Instantly, your broken files will revert to the exact pristine state they were in during your last `commit`. This is why we commit often! The more you commit, the safer you are.
