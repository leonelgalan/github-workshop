# Git Fundamentals Demo

```bash
mkdir my-project
cd my-project
git init
# "Initialized empty Git repository!"
```

```bash
# Add file and commit
git add analysis.R
git commit -m "Start analysis script"
git log --oneline
```

<!-- notes:
Do this live.
Show: init → status → add → commit → log.
Let them see how it tracks history.
-->

---

# Make a Change

```bash
# Edit analysis.R
git diff
git add analysis.R
git commit -m "Calculate mean response"
```

<!-- notes:
Show them how Git captures the *exact* change.
Magic moment: `git diff`.
-->

---

# Push to GitLab

```bash
git remote add origin https://gitlab.com/username/my-project.git
git push -u origin main
```

<!-- notes:
Show the project appear in the GitLab browser view.
Celebrate: first repo in the cloud!
-->