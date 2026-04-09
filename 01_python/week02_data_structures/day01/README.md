# Week 2 — Day 1: Lists

## 🎯 Today's Objective
Master Python's most versatile data structure. Understand ordering, indexing, and mutability.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- Creating lists: `[1, 2, 3]`
- Indexing: `list[0]`, `list[-1]`
- Slicing: `list[1:3]`, `list[::2]`
- Methods: `append()`, `extend()`, `insert()`, `remove()`, `sort()`, `reverse()`
- `len()`, `in` operator
- **Mutability** (this is critical!)

**Read one of these:**
- [Python Tutorial: Lists](https://docs.python.org/3/tutorial/datastructures.html#more-on-lists)
- [Real Python: Lists and Tuples](https://realpython.com/python-lists-tuples/)

## 💻 BUILD (30-40 min)
Create `day01_lists.py` in this folder.

**Requirements:** Process a list of warehouse shift metrics.
- Create: `shifts = [450, 380, 520, 410, 490, 440, 510, 475, 395, 530]`
- Filter out any shifts below 400 (create a new list)
- Sort the remaining shifts from highest to lowest
- Find the top 3 shifts
- Calculate the average of the top 3
- Demonstrate the **mutability trap**: assign the list to a new variable, modify it, and show both variables change

**Mutability demo:**
```python
a = [1, 2, 3]
b = a           # NOT a copy!
b.append(4)
print(a)        # [1, 2, 3, 4] — a changed too!

# The fix:
c = a.copy()    # real copy
```

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. What's the difference between `list.sort()` and `sorted(list)`?
2. Why does `b = a` NOT create a copy when `a` is a list?
3. What's the right way to copy a list?
4. When would you use `append()` vs `extend()`?

## 📦 COMMIT
```bash
git add -A
git commit -m "📦 Week 2 Day 1: Lists and mutability"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

