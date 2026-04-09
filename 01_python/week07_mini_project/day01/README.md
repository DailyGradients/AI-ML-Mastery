# Week 7 — Day 1: Define the Problem

## 🎯 Today's Objective
Scope your first real project. Create sample data.

## 📘 LEARN (15-20 min)
**No new concepts.** Today is about project planning.

**Think about:**
- What problem are you solving?
- Who is the user?
- What data do you need?
- What output do you want?

## 💻 BUILD (30-40 min)
**Project: Warehouse Shift Productivity Analyzer**

**Task 1:** Create `project_spec.md` with:
- Project name
- Problem statement
- Input format (CSV columns)
- Processing steps
- Output format
- Success criteria

**Task 2:** Create `sample_data.csv` with realistic messy data:

```csv
date,shift,employee_id,units_processed,hours_worked,errors
2026-04-01,A,EMP001,450,8.0,2
2026-04-01,A,EMP002,380,7.5,5
2026-04-01,A,EMP003,,8.0,1
2026-04-01,B,EMP004,520,8.0,bad
2026-04-02,A,EMP001,490,8.0,3
2026-04-02,A,EMP002,,,0
2026-04-02,B,EMP005,410,7.0,2
DUPLICATE ROW BELOW
2026-04-02,B,EMP005,410,7.0,2
2026-04-03,A,EMP001,530,8.0,1
```

Include: missing values, wrong types, duplicates, blank rows.

**RULES:** No pandas. No NumPy. Pure Python only.

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. Why start with a spec instead of code?
2. Why create intentionally messy data?
3. What makes a good project spec?

## 📦 COMMIT
```bash
git add -A
git commit -m "🏗️ Week 7 Day 1: Project definition"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

