# Week 7 — Day 3: Transform & Calculate

## 🎯 Today's Objective
Build the processing logic.

## 📘 LEARN (15-20 min)
**No new concepts.** Apply your knowledge.

## 💻 BUILD (30-40 min)
Create `processor.py` in this folder.

**Functions to build:**
```python
def calculate_productivity(row):
    """Units per hour for one shift."""
    pass

def shift_summary(rows):
    """Calculate overall stats: total units, avg productivity, error rate."""
    pass

def by_employee(rows):
    """Group rows by employee_id. Return dict of employee -> stats."""
    pass

def by_date(rows):
    """Group rows by date. Return dict of date -> stats."""
    pass

def top_performers(rows, n=3):
    """Return top N employees by average productivity."""
    pass

def error_analysis(rows):
    """Return employees with highest error rates."""
    pass
```

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. How did breaking the work into functions help?
2. What edge cases did you have to handle?
3. Did you need to modify your Day 2 code? Why?

## 📦 COMMIT
```bash
git add -A
git commit -m "🏗️ Week 7 Day 3: Processing and calculations"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

