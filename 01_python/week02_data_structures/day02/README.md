# Week 2 — Day 2: Dictionaries

## 🎯 Today's Objective
Learn key-value storage. Understand why dicts are the natural representation for ML data.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- Creating dicts: `{"key": "value"}`
- Access: `dict["key"]` and `dict.get("key", default)`
- Methods: `.keys()`, `.values()`, `.items()`
- Adding/updating: `dict["new_key"] = value`
- `in` operator checks keys
- Nested dictionaries

**Read one of these:**
- [Real Python: Dictionaries](https://realpython.com/python-dicts/)
- [Python Tutorial: Dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries)

## 💻 BUILD (30-40 min)
Create `day02_shift_tracker.py` in this folder.

**Requirements:** Build a shift performance tracking system using dictionaries.

```python
shifts = [
    {"id": "SH-001", "date": "2026-04-01", "supervisor": "Martinez",
     "target": 500, "actual": 487, "headcount": 12},
    {"id": "SH-002", "date": "2026-04-01", "supervisor": "Chen",
     "target": 500, "actual": 523, "headcount": 13},
    {"id": "SH-003", "date": "2026-04-02", "supervisor": "Rodriguez",
     "target": 500, "actual": 445, "headcount": 11},
]
```

**Functions to build:**
- `get_shift_by_id(shifts, shift_id)` — find and return a shift
- `shifts_over_target(shifts)` — return list of shifts that met target
- `average_productivity(shifts)` — return avg actual/headcount
- `top_supervisor(shifts)` — return supervisor with highest total actual units

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. When should you use `dict["key"]` vs `dict.get("key", default)`?
2. Why are dictionaries the natural representation for a row of data in ML?
3. What's the difference between a list of dicts and a dict of lists?

## 📦 COMMIT
```bash
git add -A
git commit -m "📦 Week 2 Day 2: Dictionaries and key-value data"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

