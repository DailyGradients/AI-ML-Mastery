# Week 6 — Day 1: Common Exceptions

## 🎯 Today's Objective
Recognize the exception types you'll see most often.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `TypeError`, `ValueError`, `KeyError`, `IndexError`
- `AttributeError`, `NameError`, `ZeroDivisionError`
- `FileNotFoundError`, `ImportError`
- How to read exception messages

**Read:**
- [Real Python: Python Exceptions](https://realpython.com/python-exceptions/)

## 💻 BUILD (30-40 min)
Create `day01_exceptions.py` in this folder.

**Task:** Intentionally trigger each exception type, then document what caused it.

```python
# TypeError: mixing incompatible types
try:
    result = "hello" + 5
except TypeError as e:
    print(f"TypeError caught: {e}")

# ValueError: right type, wrong value
try:
    num = int("not a number")
except ValueError as e:
    print(f"ValueError caught: {e}")

# KeyError: missing dict key
# IndexError: out of range
# AttributeError: method doesn't exist
# ZeroDivisionError: dividing by zero
# FileNotFoundError: file doesn't exist
```

Trigger and catch ALL of the above. Document each.

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. What's the difference between `TypeError` and `ValueError`?
2. How do you decide WHICH exception to catch?
3. What's wrong with `except:` (bare except)?

## 📦 COMMIT
```bash
git add -A
git commit -m "🐛 Week 6 Day 1: Common exceptions"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

