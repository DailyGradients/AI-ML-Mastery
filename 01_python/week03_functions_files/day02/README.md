# Week 3 — Day 2: Scope & Return Values

## 🎯 Today's Objective
Understand where variables live and die. Learn the LEGB rule.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- Local scope (inside a function)
- Global scope (module level)
- The LEGB rule: Local → Enclosing → Global → Built-in
- Why modifying globals from functions is bad
- Returning multiple values (tuples)
- `None` as a return value

**Read:**
- [Real Python: Python Scope & the LEGB Rule](https://realpython.com/python-scope-legb-rule/)

## 💻 BUILD (30-40 min)
Create `day02_scope.py` in this folder.

**Part 1: Intentionally break code with scope issues**
```python
total = 0

def add_to_total(value):
    total = total + value  # ERROR! Why?
    return total

add_to_total(10)
```

Explore what happens. Document the error.

**Part 2: Fix it properly**
Rewrite without using global variables. Pass values in, return values out.

**Part 3: Return multiple values**
```python
def analyze_shift(units, hours, target):
    """Return (productivity, status, efficiency)."""
    productivity = units / hours
    status = "met" if units >= target else "missed"
    efficiency = units / target
    return productivity, status, efficiency

# Unpack the return values
prod, stat, eff = analyze_shift(480, 8, 500)
```

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. What is the LEGB rule?
2. Why should you avoid modifying global variables from inside functions?
3. How do you return multiple values from a function in Python?
4. What does `None` mean?

## 📦 COMMIT
```bash
git add -A
git commit -m "🔧 Week 3 Day 2: Scope and return values"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

