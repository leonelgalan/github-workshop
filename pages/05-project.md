# Form Teams

**Groups of 4**, each implementing **one function** from `scripts/01_clean_data.py`

1. Pick a **team color name** from [CSS colors](https://matplotlib.org/stable/gallery/color/named_colors.html#css-colors)
2. Assess your group's **programming experience** (beginner/intermediate/advanced)
3. Send **one person** to get your assigned function

Each group submits a PR before the end of Day 1

<!-- notes:
Assign each group one of the 16 TODO functions.

Function Difficulty Guide:
⚡ Very Easy (5-10 min) - 3 functions:
  _profit, _is_profitable, _to_millions

✅ Easy (15-20 min) - 4 functions:
  _budget_category, _vote_count_bucket, _runtime_bucket, _log1p_nonnegative

🟡 Medium (25-35 min) - 6 functions:
  _decade_label, _greater_than_zero, _extract_director, _take_first,
  _names_from_json, _revenue_to_budget_ratio

🟠 Medium-Hard (35-50 min) - 3 functions:
  _pick_if_present, _roi, _codes_from_json

⚠️ Key Notes:
- Factory functions (_codes_from_json, _pick_if_present, _take_first) return functions
- _codes_from_json is the hardest (factory + closure)
- Assign easier functions to less experienced groups
-->

---
layout: image
image: ./pages/colors.png
backgroundSize: contain
---

<!--
Team Colors: https://matplotlib.org/stable/gallery/color/named_colors.html#css-colors
-->

---

# Fork & Clone Project

1. Fork `https://github.com/leonelgalan/movie-analysis`
2. Clone your fork locally

```bash
git clone https://github.com/YOUR-USERNAME/movie-analysis.git
code movie-analysis .
```

<!-- notes:
Each group forks the repo to their own account.
They'll submit PRs from their fork back to the main repo.
-->

---

# Configure Identity

```bash
git config --global user.name "Your Name"
git config --global user.email "you@ncsu.edu"
git config --global init.defaultBranch main
```

<!-- notes:
Tedious but essential.
Check with `git config --list`.
-->

---

# Class Activity: Implement Your Function

1. Create a feature branch
2. Implement your assigned function in `scripts/01_clean_data.py`
3. Test it works (run the script)
4. Commit and push to your fork
5. Submit a PR to the main repo

```bash
git checkout -b implement-your-function-name
# ... edit the file ...
git add scripts/01_clean_data.py
git commit -m "Implement _your_function_name"
git push origin implement-your-function-name
```

<!-- notes:
Walk through the workflow once as a class.
Help groups with their specific function logic.
Ensure everyone submits a PR before leaving.
-->

---

# Between Sessions

1. **Pull the latest changes** from the main repo after all PRs are merged.
2. **Complete your assigned script** (`02`, `03`, or `04`) — see
   `docs/PROJECT_SPEC.md` for details.
3. **Commit early and often** as you make progress.
4. **Push your work** before Day 2.

**Bonus challenge:**
Try bringing work from another team’s repository — just like in open source.
To do this, you’ll need to experiment with adding a new Git remote and merging
(or cherry-picking) their changes into your project. If you do, make sure
everything runs cleanly end-to-end afterward.

<!-- notes:
By the end of today, all 16 functions will be merged into main.
Between sessions, students work independently on their assigned analysis scripts.
Encourage curiosity: exploring remotes and merging others' work is optional, but
gives a taste of real-world open-source collaboration. Next session: we'll focus
on integrating everyone’s analysis and resolving merge conflicts.
-->

---

# Day 2: Merge & Report

- Merge everyone's analysis work
- Resolve merge conflicts together
- Prepare a final report
- Celebrate completed collaboration!

<!-- notes:
Day 2 is about integration and conflict resolution.
Work through merge conflicts as teaching moments.
End with a summary report showing combined results.
-->
