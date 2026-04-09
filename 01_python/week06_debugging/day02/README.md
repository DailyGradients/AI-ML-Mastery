# Week 6 — Day 2: Reading Stack Traces

## 🎯 Today's Objective
Learn to read error messages calmly and find the bug.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- How to read a traceback (bottom up!)
- The call stack
- Finding the line that actually caused the error
- Error propagation through function calls

**Read:**
- [Real Python: Python Traceback](https://realpython.com/python-traceback/)

## 💻 BUILD (30-40 min)
Create a multi-file project that generates a stack trace.

**Create these 3 files:**

`main.py`:
```python
from processor import process_shift

data = {"units": "500", "hours": 0}
result = process_shift(data)
print(result)
```

`processor.py`:
```python
from utils import calculate_rate

def process_shift(data):
    units = int(data["units"])
    hours = data["hours"]
    rate = calculate_rate(units, hours)
    return rate
```

`utils.py`:
```python
def calculate_rate(units, hours):
    return units / hours  # ZeroDivisionError!
```

**Task:**
1. Run `main.py` and see the traceback
2. Read it from BOTTOM to TOP
3. In a file called `trace_analysis.md`, document:
   - What type of error
   - Which file/line
   - The chain of calls
   - How to fix it

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. Why read tracebacks from bottom to top?
2. What information does a traceback give you?
3. How would you fix the bug in the example?

## 📦 COMMIT
```bash
git add -A
git commit -m "🐛 Week 6 Day 2: Reading tracebacks"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

