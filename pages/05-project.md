# Before We Start

Ensure you have:

- ✅ GitHub account created
- ✅ Git installed locally
- ✅ VS Code installed
- ✅ Basic terminal/command line familiarity

**Quick check:**

```bash
git --version
code --version
```

<!-- notes:
Do a quick show of hands to catch anyone missing prerequisites.
Have backup plans for common issues.
-->

---

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
code movie-analysis
```

## Why fork?

- You get your own copy to experiment safely
- Submit changes back via Pull Requests
- Practice open-source contribution workflow

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

# Testing Your Function

Before committing, verify your function works:

```bash
uv run python scripts/01_clean_data.py
uv run pytest -k your_function_name
```

Look for:

- ✅ No error messages
- ✅ Script completes successfully
- ✅ Output file `results/movies_clean.csv` created

<!-- notes:
Emphasize testing BEFORE pushing.
Show how to read error messages if something fails.
-->

---

# Between Sessions

1. Sync with upstream (all 16 functions now available!)

   ```bash
   git remote add upstream https://github.com/leonelgalan/movie-analysis.git
   git pull upstream main
   ```

2. **Collaborate to complete all analysis scripts** (`02`, `03`, `04`)
   - Work together or divide the scripts among team members
   - OR pull completed scripts from other teams' repos (like open source!)
3. Create feature branches and commit frequently
4. **Open PRs within your fork** (not to upstream) for team review

**Learning opportunity:**

Practice adding remotes and merging/cherry-picking work from other teams.
This mirrors real open-source collaboration!

<!-- notes:
By the end of today, all 16 functions will be merged into main.
Between sessions, students work independently on their assigned analysis scripts.
Encourage curiosity: exploring remotes and merging others' work is optional, but
gives a taste of real-world open-source collaboration. Next session: we'll focus
on integrating everyone's analysis and resolving merge conflicts.
-->

---

# Day 2: Integration & Conflict Resolution

1. Sync with upstream changes
2. **Merge any remaining PRs within your fork**
3. **Practice conflict resolution:**
   - Two team members edit same section of `REPORT.md` on different branches
   - Create competing PRs within fork
   - Resolve merge conflict in VS Code together
4. Run complete pipeline end-to-end
5. Review results and celebrate!

<!-- notes:
Day 2 is about integration and conflict resolution WITHIN each team's fork.
Work through merge conflicts as teaching moments.
Emphasize that all PRs for scripts 02-04 are fork-internal, not to upstream.
End with a summary report showing combined results.
-->
