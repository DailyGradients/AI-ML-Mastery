# Week 5 — Day 1: List Comprehensions

## 🎯 Today's Objective
Learn the most distinctive Pythonic pattern.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- Basic comprehension: `[x*2 for x in numbers]`
- With filter: `[x for x in numbers if x > 0]`
- Nested: `[(x, y) for x in list1 for y in list2]`
- Dict comprehensions: `{k: v for k, v in pairs}`
- Set comprehensions: `{x for x in items}`

**Read:**
- [Real Python: List Comprehensions](https://realpython.com/list-comprehension-python/)

## 💻 BUILD (30-40 min)
Create `day01_comprehensions.py` in this folder.

**Task:** Rewrite these 5 loops as list comprehensions:

```python
# 1. Double every number
numbers = [1, 2, 3, 4, 5]
doubled = []
for n in numbers:
    doubled.append(n * 2)

# 2. Filter positive numbers
nums = [-3, -1, 0, 2, 5, -2, 7]
positive = []
for n in nums:
    if n > 0:
        positive.append(n)

# 3. Convert dict to list of tuples
shift_data = {"mon": 450, "tue": 520, "wed": 480}
pairs = []
for day, units in shift_data.items():
    pairs.append((day, units))

# 4. Extract uppercase names
names = ["alice", "bob", "charlie"]
upper = []
for name in names:
    upper.append(name.upper())

# 5. Shifts that hit target
shifts = [{"id": 1, "units": 450, "target": 500},
          {"id": 2, "units": 520, "target": 500}]
met = []
for shift in shifts:
    if shift["units"] >= shift["target"]:
        met.append(shift["id"])
```

For each, write BOTH the loop version and the comprehension version. Compare readability.

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. When is a comprehension MORE readable than a loop?
2. When is a comprehension LESS readable than a loop?
3. What's the rule of thumb for when to use each?

## 📦 COMMIT
```bash
git add -A
git commit -m "✨ Week 5 Day 1: List comprehensions"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

