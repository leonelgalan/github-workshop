---
layout: image
image: ./pages/filename.jpg
backgroundSize: contain
---

---
layout: image
image: ./pages/final.gif
backgroundSize: contain
---

# Why Git?

<!-- notes:
Pause for laughs.
Interactive Qs:
- Raise your hand if you have a folder like this.
- Keep it up if you’ve emailed yourself code at 2 AM.
- Keep it up if you’ve asked: which version had that graph?
Punchline: “This cartoon is from 2012. It’s 2025. We’re still doing this.”

https://www.instagram.com/p/Cz04wRdNP6_/
https://phdcomics.com/comics/archive.php?comicid=1531
-->

---

# Without Git vs With Git

❌ Without Git  

```txt
analysis_march15.R
analysis_march16.R
analysis_march16_evening.R
analysis_final_use_this_one.R
```

✅ With Git

```bash
$ git log --oneline
7a3b2c1 Fix outlier removal to 2.5 SD
6d4f8a2 Add gender as covariate
```

<!-- notes:
Emphasize: Git gives you the *story* of your project.
Not just backup: accountability, timeline, exact changes, reasons.
-->

---

# Real Project Example

```bash
git log --grep="threshold"
# Commit 7a3b2c1: "Fix outlier threshold from 3 → 2.5 SD
# Based on Cook's distance analysis showing 3 SD too permissive"
```

<!-- notes:
Set up scenario: 6 months later, reviewer #2 asks about your threshold.
Without Git: “I think it was because… let me check my notes…”
With Git: exact commit, exact reasoning.
Git protects your team's memory.
-->
