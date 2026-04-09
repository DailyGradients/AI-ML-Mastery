# Week 2 — Day 3: Sets

## 🎯 Today's Objective
Learn about unique collections and set operations.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- Creating sets: `{1, 2, 3}` or `set([1, 2, 3])`
- Automatic deduplication (duplicates silently ignored)
- Set operations: `|` (union), `&` (intersection), `-` (difference)
- `in` operator (very fast membership testing)
- Sets are **unordered** (no indexing!)
- `frozenset` (immutable version)

**Read one of these:**
- [Real Python: Sets](https://realpython.com/python-sets/)
- [Python Tutorial: Sets](https://docs.python.org/3/tutorial/datastructures.html#sets)

## 💻 BUILD (30-40 min)
Create `day03_crew_analysis.py` in this folder.

**Requirements:** Analyze warehouse crew attendance using sets.

```python
monday_crew = ["EMP001", "EMP002", "EMP003", "EMP001", "EMP004", "EMP005"]
tuesday_crew = ["EMP003", "EMP004", "EMP005", "EMP006", "EMP007", "EMP003"]
wednesday_crew = ["EMP001", "EMP005", "EMP006", "EMP008", "EMP009"]
```

**Tasks:**
- De-duplicate each day's crew list using sets
- Find employees who worked all three days (intersection)
- Find employees who worked only Monday (difference)
- Find all unique employees across all days (union)
- Count total unique employees
- Identify employees who worked exactly 2 of the 3 days

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. Why are sets unordered? When is this a problem?
2. Why is `"EMP001" in my_set` faster than `"EMP001" in my_list`?
3. What's the difference between `set()` and `frozenset()`?

## 📦 COMMIT
```bash
git add -A
git commit -m "📦 Week 2 Day 3: Sets and unique collections"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

