# Week 3 — Day 5: Modules & Refactoring

## 🎯 Today's Objective
Organize code across multiple files. Learn imports.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- Modules = Python files that can be imported
- `import module` and `from module import function`
- `if __name__ == "__main__":`
- Package structure
- Why splitting code into modules matters

**Read:**
- [Real Python: Python Modules and Packages](https://realpython.com/python-modules-packages/)

## 💻 BUILD (30-40 min)
**Task:** Refactor your Day 3/4 code into multiple files.

Create these files in `day05/`:
1. `utils.py` — helper functions (calculate_productivity, format_currency, etc.)
2. `loader.py` — the file loading functions with logging
3. `logger_config.py` — the logging setup code
4. `main.py` — ties everything together

**main.py should look like:**
```python
from logger_config import setup_logging
from loader import load_shifts
from utils import calculate_productivity, format_currency

def main():
    setup_logging()
    shifts = load_shifts("sample_shifts.csv")
    for shift in shifts:
        productivity = calculate_productivity(shift['units'], 8)
        print(f"{shift['supervisor']}: {productivity} units/hr")

if __name__ == "__main__":
    main()
```

## ✍🏽 EXPLAIN (10-15 min)
Create `../../../reflections/week03.md` and answer:
1. Why split code into multiple files?
2. What does `if __name__ == "__main__":` do?
3. What was hardest about this week?
4. Confidence level 1-10 for functions and files?

## 📦 COMMIT
```bash
git add -A
git commit -m "🔧 Week 3 Complete: Functions and files mastered"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

