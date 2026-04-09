# Week 6 — Day 5: pdb Debugger

## 🎯 Today's Objective
Use Python's built-in debugger instead of print statements.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `breakpoint()` — start debugging
- pdb commands: `n` (next), `s` (step), `c` (continue), `p` (print)
- `l` (list), `q` (quit), `h` (help)
- Setting breakpoints
- Inspecting variables

**Read:**
- [Real Python: Python Debugging with pdb](https://realpython.com/python-debugging-pdb/)

## 💻 BUILD (30-40 min)
Create `day05_pdb_session.py` in this folder.

**Task:** Debug a complex script using ONLY pdb (no print statements).

```python
def process_shifts(shifts):
    results = []
    for i, shift in enumerate(shifts):
        breakpoint()  # Pauses here!
        productivity = shift['units'] / shift['hours']
        results.append({
            'shift_num': i + 1,
            'productivity': productivity
        })
    return results

shifts = [
    {'units': 450, 'hours': 8},
    {'units': 520, 'hours': 8},
    {'units': 400, 'hours': 0},  # BUG: division by zero!
]

results = process_shifts(shifts)
print(results)
```

**At each breakpoint, practice:**
- `p shift` — print the current shift
- `p i` — print the index
- `n` — go to next line
- `c` — continue to next breakpoint
- `q` — quit

**Document your debugging session** in `debugging_notes.md`.

## ✍🏽 EXPLAIN (10-15 min)
Create `../../../reflections/week06.md` and answer:
1. When is pdb better than print statements?
2. What's your calm debugging process now?
3. Confidence level 1-10 for debugging?

## 📦 COMMIT
```bash
git add -A
git commit -m "🐛 Week 6 Complete: Debugging without spiraling"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

