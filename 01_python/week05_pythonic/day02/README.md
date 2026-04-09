# Week 5 — Day 2: zip & enumerate

## 🎯 Today's Objective
Master two essential built-in functions.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `zip(list1, list2)` — pair items from two lists
- `enumerate(list)` — get (index, value) pairs
- `dict(zip(keys, values))` — build a dict from two lists
- Why `enumerate` beats `range(len(list))`

**Read:**
- [Real Python: zip() Function](https://realpython.com/python-zip-function/)
- [Real Python: enumerate()](https://realpython.com/python-enumerate/)

## 💻 BUILD (30-40 min)
Create `day02_zip_enum.py` in this folder.

**Task 1: Parallel processing with zip**
```python
names = ["Chen", "Rodriguez", "Okafor", "Kim"]
scores = [92, 87, 95, 88]
shifts = ["morning", "evening", "night", "morning"]

# Using zip, print a report:
# 1. Chen scored 92 on morning shift
# 2. Rodriguez scored 87 on evening shift
# ...
```

**Task 2: Replace `range(len())` with enumerate**
```python
# BAD: non-Pythonic
items = ["apple", "banana", "cherry"]
for i in range(len(items)):
    print(f"{i+1}. {items[i]}")

# GOOD: Pythonic
for i, item in enumerate(items, start=1):
    print(f"{i}. {item}")
```

**Task 3: Build a dict from two lists**
```python
headers = ["date", "supervisor", "units"]
row = ["2026-04-01", "Martinez", 487]

# Use dict(zip()) to create: {"date": "2026-04-01", ...}
```

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. Why is `enumerate()` better than `range(len())`?
2. What happens when you `zip()` lists of different lengths?
3. How can `zip()` and `dict()` work together?

## 📦 COMMIT
```bash
git add -A
git commit -m "✨ Week 5 Day 2: zip and enumerate"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

