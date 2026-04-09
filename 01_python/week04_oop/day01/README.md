# Week 4 — Day 1: Classes & Objects

## 🎯 Today's Objective
Understand the class/object blueprint pattern.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- Classes as blueprints
- Objects as instances of classes
- `class` keyword
- Attributes (data)
- Creating instances: `obj = ClassName()`

**Read one of these:**
- [Real Python: OOP in Python](https://realpython.com/python3-object-oriented-programming/)
- [Corey Schafer: OOP Basics (YouTube)](https://www.youtube.com/watch?v=ZDa-Z5JzLYM)

## 💻 BUILD (30-40 min)
Create `day01_employee.py` in this folder.

**Build an Employee class:**
```python
class Employee:
    def __init__(self, name, role, hourly_rate):
        self.name = name
        self.role = role
        self.hourly_rate = hourly_rate
        self.shift_hours = []  # starts empty

    def log_shift(self, hours):
        self.shift_hours.append(hours)

    def total_hours(self):
        return sum(self.shift_hours)

    def weekly_pay(self):
        return self.total_hours() * self.hourly_rate
```

**Test it:**
- Create 3 different employees
- Log shifts for each
- Print their weekly pay
- Print each employee's total hours

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. What's the difference between a class and an object?
2. What does `self` mean in a method?
3. Why does `__init__` get called automatically?
4. What makes OOP different from just using functions?

## 📦 COMMIT
```bash
git add -A
git commit -m "🏗️ Week 4 Day 1: Classes and objects"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

