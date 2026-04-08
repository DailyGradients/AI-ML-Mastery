# Week 1 — Day 2: Conditionals

## 🎯 Today's Objective
Control the flow of your programs with decisions. Learn how if/elif/else statements work.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `if`, `elif`, `else` statements
- Comparison operators: `==`, `!=`, `<`, `>`, `<=`, `>=`
- Logical operators: `and`, `or`, `not`
- Truthiness (what counts as True or False)
- Indentation in Python (4 spaces, always)

**Read one of these:**
- [Automate the Boring Stuff Ch 2](https://automatetheboringstuff.com/2e/chapter2/) — Flow Control
- [Real Python: Conditional Statements](https://realpython.com/python-conditional-statements/)

## 💻 BUILD (30-40 min)
Create `day02_shipping_calculator.py` in this folder.

**Requirements:** Build a shipping cost calculator for a warehouse.
- Ask user for package weight (in pounds)
- Ask user for destination zone (A, B, or C)
- Calculate cost based on:
  - Zone A: $5.00 base + $0.50/lb
  - Zone B: $8.00 base + $0.75/lb
  - Zone C: $12.00 base + $1.00/lb
- Add 10% surcharge for packages over 50 lbs
- Print a formatted invoice

**Starter code:**
```python
weight = float(input("Package weight (lbs): "))
zone = input("Zone (A/B/C): ").upper()

if zone == "A":
    cost = 5.00 + (weight * 0.50)
elif zone == "B":
    cost = 8.00 + (weight * 0.75)
# ... continue
```

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. What happens if your `if/elif` chain doesn't cover all possible inputs?
2. Why is indentation so important in Python?
3. What's a "silent failure" and why is it dangerous?

## 📦 COMMIT
```bash
git add -A
git commit -m "🐍 Week 1 Day 2: Conditionals and decision logic"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

