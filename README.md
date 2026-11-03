# Python Interactive Workbook

Personal workspace for learning Python while working through *Python Crash Course* (3rd Edition) by Eric Matthes.

This is a simple place to keep exercises, notes, and small projects as you go. It starts with the chapter you're currently working on and grows only as you need it.

## Purpose
- Practice the exercises from the book
- Keep your own notes and takeaways
- Track what you've actually completed
- Stay organized without extra complexity

## Setup

### 1. Create a virtual environment
From the root of this repository:

```bash
python -m venv .venv
```

### 2. Activate it
- **Windows (Command Prompt):** `.venv\Scripts\activate`
- **Windows (PowerShell):** `.venv\Scripts\Activate.ps1`
- **macOS / Linux:** `source .venv/bin/activate`

When it's active, your prompt will usually show `(.venv)`.

### 3. Install dependencies (when needed)
Right now there are none. When an exercise needs a third-party package, install it with:

```bash
pip install package-name
```

Then note it in this README under a short "Dependencies" section so you remember later.

## How to run Python files
From the root of the repo (with your virtual environment activated):

```bash
python chapters/chapter_02/example.py
```

Or navigate into a folder and run the file directly.

## Current structure
```
chapters/
  chapter_02/
    exercises/     ← put your exercise attempts here
    notes/         ← notes, questions, and takeaways
    example.py     ← small runnable example to verify setup
```

## Progress checklist

Update this as you actually finish work — not just because a file exists.

### Part I: Basics
- [ ] Chapter 1: Getting Started
- [ ] Chapter 2: Variables and Simple Data Types ← **current**
- [ ] Chapter 3: Introducing Lists
- [ ] Chapter 4: Working with Lists
- [ ] Chapter 5: if Statements
- [ ] Chapter 6: Dictionaries
- [ ] Chapter 7: User Input and while Loops
- [ ] Chapter 8: Functions
- [ ] Chapter 9: Classes
- [ ] Chapter 10: Files and Exceptions
- [ ] Chapter 11: Testing Your Code

### Part II: Projects
- [ ] Chapter 12: A Ship That Fires Bullets
- [ ] Chapter 13: Aliens!
- [ ] Chapter 14: Scoring
- [ ] Chapter 15: Generating Data
- [ ] Chapter 16: Downloading Data
- [ ] Chapter 17: Working with APIs
- [ ] Chapter 18: Getting Started with Django
- [ ] Chapter 19: User Accounts
- [ ] Chapter 20: Styling and Deploying an App

## Next study session
1. Activate the virtual environment
2. Open `chapters/chapter_02/example.py` and run it
3. Start your Chapter 2 exercises in `chapters/chapter_02/exercises/`
4. Record any notes or questions in `chapters/chapter_02/notes/`
