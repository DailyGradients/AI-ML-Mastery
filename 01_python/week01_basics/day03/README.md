# Week 1 — Day 3: Loops

## 🎯 Today's Objective
Repeat operations over collections of data. Master for loops and while loops.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `for` loops (iterate over a collection)
- `while` loops (repeat while a condition is true)
- `range()` function
- `break` and `continue`
- Loop counters and accumulators

**Read one of these:**
- [Real Python: For Loops](https://realpython.com/python-for-loop/)
- [Automate the Boring Stuff Ch 2 (loops section)](https://automatetheboringstuff.com/2e/chapter2/)

## 💻 BUILD (30-40 min)
Create `day03_aggregator.py` in this folder.

**Requirements:** Process a list of shift productivity numbers without using built-in functions like `sum()` or `max()`.
- Create a list: `shifts = [450, 380, 520, 410, 490, 440, 510, 475, 395, 530]`
- Use a for loop to calculate:
  - Total units
  - Average units per shift
  - Maximum shift
  - Minimum shift
  - Count of shifts above 450
- Print a summary report

**Starter code:**
```python
shifts = [450, 380, 520, 410, 490, 440, 510, 475, 395, 530]
total = 0
maximum = shifts[0]
minimum = shifts[0]

for value in shifts:
    total += value
    if value > maximum:
        maximum = value
    # ... continue
```

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. What's the difference between a `for` loop and a `while` loop?
2. What does `range(5)` produce? Why does Python start counting at 0?
3. Why will loops over large datasets be slow in pure Python?

## 📦 COMMIT
```bash
git add -A
git commit -m "🐍 Week 1 Day 3: Loops and iteration"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

