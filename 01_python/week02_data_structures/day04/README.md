# Week 2 — Day 4: Compare All Three

## 🎯 Today's Objective
Understand when to use list vs dict vs set. Build a decision framework.

## 📘 LEARN (15-20 min)
**No new concepts.** Today is about choosing the right tool.

**Decision framework:**
- **List**: ordered, allows duplicates, access by position
- **Dict**: key-value pairs, fast lookup by name
- **Set**: unique items, fast membership testing, no order

**Read:**
- [Real Python: Common Python Data Structures](https://realpython.com/python-data-structures/)

## 💻 BUILD (30-40 min)
Create `day04_three_ways.py` in this folder.

**Task:** Given the same problem, solve it three different ways.

**Problem:** Given 1000 employee IDs with duplicates, find unique IDs and count how many times each one appears.

```python
import random
ids = [f"EMP{random.randint(1, 200):03d}" for _ in range(1000)]
```

**Solution 1 (using a list):**
- Loop through IDs
- Keep a list of seen IDs
- For each new ID, check if it's already in the seen list

**Solution 2 (using a dict):**
- Loop through IDs
- Use a dict where keys are IDs and values are counts

**Solution 3 (using a set):**
- Use `set()` to get unique IDs
- Then count (but note: sets don't count!)

Time each approach using `import time; start = time.time()`. Which is fastest?

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` with a **decision framework**:
- "If I need ____, I should use ____"
- Write at least 5 rules based on what you learned
- Which approach was fastest? Why?

## 📦 COMMIT
```bash
git add -A
git commit -m "📦 Week 2 Day 4: Comparing data structures"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

