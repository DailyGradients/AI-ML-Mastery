# Week 3 — Day 1: Functions & Arguments

## 🎯 Today's Objective
Write reusable, modular code. Learn the unit of reusability in programming.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `def` keyword to define functions
- Parameters vs arguments
- `return` statements
- Default parameter values
- Positional vs keyword arguments
- Docstrings (`"""description"""`)

**Read one of these:**
- [Real Python: Defining Functions](https://realpython.com/defining-your-own-python-function/)
- [Python Tutorial: Defining Functions](https://docs.python.org/3/tutorial/controlflow.html#defining-functions)

## 💻 BUILD (30-40 min)
Create `day01_functions.py` in this folder.

**Build these functions:**

```python
def calculate_productivity(units, hours):
    """Calculate units per hour."""
    if hours <= 0:
        return 0
    return round(units / hours, 2)

def format_currency(amount, symbol="$", decimals=2):
    """Format a number as currency."""
    return f"{symbol}{amount:,.{decimals}f}"

def classify_performance(rate, threshold=55):
    """Classify a productivity rate as high/medium/low."""
    if rate >= threshold:
        return "high"
    elif rate >= threshold * 0.8:
        return "medium"
    else:
        return "low"
```

**Then use them together:**
- Process at least 5 shifts
- For each shift, calculate productivity, classify it, and print a formatted report

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. What's the difference between `print()` and `return`?
2. Why are default parameter values useful?
3. What makes a good function name?
4. How do functions make code reusable?

## 📦 COMMIT
```bash
git add -A
git commit -m "🔧 Week 3 Day 1: Functions and arguments"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

