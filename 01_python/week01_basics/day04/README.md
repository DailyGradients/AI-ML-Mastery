# Week 1 — Day 4: Input/Output

## 🎯 Today's Objective
Get data in and out of your programs. Learn string formatting with f-strings.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `input()` function (returns a string!)
- `print()` function
- F-strings: `f"Hello, {name}"`
- Format specifiers: `f"{value:.2f}"`, `f"${value:,.2f}"`
- Type conversion with `int()`, `float()`

**Read one of these:**
- [Real Python: F-Strings](https://realpython.com/python-f-strings/)
- [Python Tutorial: Input/Output](https://docs.python.org/3/tutorial/inputoutput.html)

## 💻 BUILD (30-40 min)
Create `day04_shift_calculator.py` in this folder.

**Requirements:** Interactive warehouse shift pay calculator.
- Ask user for:
  - Employee name
  - Hours worked
  - Hourly rate
  - Shift type (day/evening/night)
- Apply shift premium:
  - Day: no premium
  - Evening: 10% premium
  - Night: 15% premium
- Calculate and display total pay with nice formatting
- Handle overtime (anything over 40 hours) at 1.5x rate

**Starter code:**
```python
name = input("Employee name: ")
hours = float(input("Hours worked: "))
rate = float(input("Hourly rate: $"))
shift = input("Shift (day/evening/night): ").lower()

# Calculate base pay with premium
# Handle overtime
# Print formatted result
print(f"{name} earned: ${total_pay:,.2f}")
```

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. Why does `input()` always return a string, even if the user types a number?
2. Why does production ML code never use `input()`?
3. What are 3 useful f-string format specifiers?

## 📦 COMMIT
```bash
git add -A
git commit -m "🐍 Week 1 Day 4: Input/output and f-strings"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

