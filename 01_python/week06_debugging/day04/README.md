# Week 6 — Day 4: Bug Safari

## 🎯 Today's Objective
Intentionally break code, then fix it. Build debugging intuition.

## 📘 LEARN (15-20 min)
**No new concepts.** Today you practice debugging.

## 💻 BUILD (30-40 min)
**Task: Take a working script and introduce 10 bugs. Then fix them.**

Start with this working code:
```python
def calculate_shift_metrics(shifts):
    total_units = 0
    total_hours = 0
    for shift in shifts:
        total_units += shift['units']
        total_hours += shift['hours']

    avg_productivity = total_units / total_hours
    return {
        'total_units': total_units,
        'total_hours': total_hours,
        'avg_productivity': round(avg_productivity, 2)
    }

shifts = [
    {'units': 450, 'hours': 8},
    {'units': 520, 'hours': 8},
    {'units': 480, 'hours': 7.5},
]

result = calculate_shift_metrics(shifts)
print(result)
```

**Save the buggy versions as `bug_01.py`, `bug_02.py`, etc.**

**Bugs to introduce (one per file):**
1. Typo in variable name
2. Off-by-one error
3. Wrong operator (`*` instead of `+`)
4. Missing return
5. Wrong dict key
6. Integer division issue
7. Trying to access non-existent key
8. Infinite loop
9. Wrong indentation
10. Division by zero possibility

**Document each:** what you did, what error it caused, and the fix.

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. Which bug was hardest to find? Why?
2. What's your debugging process now?
3. How do you stay calm when you see an error?

## 📦 COMMIT
```bash
git add -A
git commit -m "🐛 Week 6 Day 4: Bug safari"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

