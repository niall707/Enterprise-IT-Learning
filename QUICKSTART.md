# Quickstart — Put This Repository on GitHub

These steps are for an ordinary **local Git repository** on Windows, using VS Code and a GitHub repository you own.

## Recommended local folder

Use a normal working directory such as `C:\Projects\enterprise-it-learning` rather than a OneDrive-synchronised folder. Git controls version history; simultaneous OneDrive sync of `.git` can introduce conflicts.

## Option A — You have not created the GitHub repository yet

1. Create a **new empty** GitHub repository called `enterprise-it-learning` (leave GitHub's README/gitignore/licence initialization unchecked).
2. Extract the contents of `Enterprise_IT_Learning_GitHub_Starter.zip` so `README.md` sits at the top of the local `enterprise-it-learning` folder (not in an extra nested folder).
3. Open a terminal **inside that folder**, then run:

```powershell
git init
git add .
git commit -m "Initial Enterprise IT Learning framework"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/enterprise-it-learning.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your real GitHub handle. Authentication is handled by Git/Git Credential Manager or GitHub CLI; never paste a token into tracked files.

## Option B — The GitHub repository already exists

1. Clone it to your local working folder:

```powershell
cd C:\Projects
git clone https://github.com/YOUR-USERNAME/enterprise-it-learning.git
```

2. Copy the files **inside** the downloaded starter folder into the cloned `enterprise-it-learning` folder. Do not copy an extra `.git` directory or overwrite work without reviewing changes.
3. From inside the clone:

```powershell
git status
git add .
git commit -m "Add learning framework and templates"
git push
```

If Git reports 'nothing to commit', confirm that the starter files are in the repository directory. If your existing files conflict, compare them before merging.

## First real entry

1. Open [01-systems-administration/rhel](01-systems-administration/rhel/README.md).
2. Copy `templates/course-notes-template.md` into that folder with a meaningful name, for example `systemd-course-notes.md`.
3. After practising on a personally controlled lab VM, use `templates/lab-report-template.md` to document real results.
4. Link your note and lab from [PROGRESS-TRACKER.md](PROGRESS-TRACKER.md).

## Before pushing any update

Read [SECURITY.md](SECURITY.md), check `git diff --staged`, and verify no sensitive workplace data is present.
