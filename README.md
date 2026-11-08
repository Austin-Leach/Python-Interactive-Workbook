# Python Interactive Workbook

Personal workspace for learning Python with *Python Crash Course* (3rd Edition) by Eric Matthes.

Use the book as the reference, an AI tutor for short explanations and feedback, and VS Code to write and run your own code. This repository keeps your work and study checkpoint available across computers.

## Start here

1. Read [PROGRESS.md](PROGRESS.md) for the latest recorded checkpoint.
2. Give your tutor [TUTOR_INSTRUCTIONS.md](TUTOR_INSTRUCTIONS.md), your progress file, and the relevant code.
3. Work through one small concept and exercise at a time.
4. Run your attempt in VS Code, review the result, and record what you learned.
5. Commit and push your changes before switching computers.

The existing scaffold starts at Chapter 2. That is an organizational starting point, not evidence of completed learning.

## Set up on each computer

Install Python 3, Git, VS Code, and the VS Code Python extension. Clone this repository once on each computer, then open its folder in VS Code:

```bash
git clone https://github.com/Austin-Leach/Python-Interactive-Workbook.git
cd Python-Interactive-Workbook
python -m venv .venv
```

If Windows does not recognize `python`, use `py` to create the environment.

Activate it:
- Windows PowerShell: `.\.venv\Scripts\Activate.ps1`
- Windows Command Prompt: `.venv\Scripts\activate.bat`
- macOS / Linux: `source .venv/bin/activate`

In VS Code, run **Python: Select Interpreter** and choose this repository's `.venv`. Create a separate environment on each computer; it is not synced through Git.

Run the existing setup example from the repository root:

```bash
python chapters/chapter_02/example.py
```

If PowerShell blocks activation, you can run it directly:
```powershell
.\.venv\Scripts\python.exe chapters/chapter_02/example.py
```

No third-party dependencies are currently needed. Add packages only when a chapter requires them, using `python -m pip install package-name`, and record the actual package and version in that chapter's notes.

## Workbook structure

```text
README.md
PROGRESS.md
TUTOR_INSTRUCTIONS.md
chapters/
  chapter_02/
    example.py
    exercises/
      README.md
    notes/
      notes.md
```

Keep exercise attempts in the existing exercises folder, for example `2-1_simple_message.py`. Use the book's exercise numbers. Save explanations, questions, and takeaways in the chapter's notes. Add `chapter_03/exercises/` and `chapter_03/notes/notes.md` only when you reach that chapter; repeat as needed. No empty full-book scaffold or prewritten solutions are required.

## A study session

- Read the relevant section, then ask for the essential idea, a tiny example, and one practice task.
- Write your own attempt before requesting a solution.
- Run it, compare actual and expected output, and share the code and exact error if stuck.
- Ask for a hint first; explain the working solution in your own words.
- Update [PROGRESS.md](PROGRESS.md) with the exact next action and any unresolved question. Mark completion only when supported by your actual work.

## Continue on another computer

Before starting, from the repository folder:

```bash
git status
git pull --ff-only
```

Finish or commit local changes before pulling. If Git reports a conflict or divergent history, resolve it before continuing; do not discard work or force-push to get past it.

At the end of a session:

```bash
git status
git diff
git add chapters/ PROGRESS.md
git commit -m "Practice chapter 2 exercises and record next step"
git push
```

Use a message that describes what you actually did. Stage any intentionally edited guide files separately. Pushing sends committed files to GitHub; the other computer receives them after pulling.

## Starting or resuming tutoring

Copy this into your tutoring chat and provide the referenced files:

> Follow TUTOR_INSTRUCTIONS.md. Read PROGRESS.md and my relevant exercise files. Use my copy of Python Crash Course as the reference when available. Resume from the recorded next action, teach the essentials concisely, and give me one task to attempt in VS Code. Ask for missing context instead of inventing progress or exercise wording.

The saved progress file is the handoff between sessions. Provide its latest version and relevant code whenever the tutor cannot access the repository.

Keep the full book and other private reference material out of this public repository. Store your own code and notes here.
