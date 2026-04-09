# Week 5 — Day 5: Custom Iterators

## 🎯 Today's Objective
Understand the iterator protocol. Build your own.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `__iter__` and `__next__` methods
- The iterator protocol
- `StopIteration` exception
- Why `for` loops work with any iterator

**Read:**
- [Real Python: Python Iterators](https://realpython.com/python-iterators-iterables/)

## 💻 BUILD (30-40 min)
Create `day05_iterator.py` in this folder.

**Build a ShiftSchedule iterator:**
```python
class ShiftSchedule:
    """Iterates through shifts in a rotation."""

    def __init__(self, shifts, max_rotations=None):
        self.shifts = shifts
        self.max_rotations = max_rotations
        self.current_index = 0
        self.rotations = 0

    def __iter__(self):
        return self

    def __next__(self):
        if self.max_rotations and self.rotations >= self.max_rotations:
            raise StopIteration

        shift = self.shifts[self.current_index]
        self.current_index += 1

        if self.current_index >= len(self.shifts):
            self.current_index = 0
            self.rotations += 1

        return shift

# Use it
schedule = ShiftSchedule(["morning", "evening", "night"], max_rotations=2)
for shift in schedule:
    print(shift)
```

## ✍🏽 EXPLAIN (10-15 min)
Create `../../../reflections/week05.md` and answer:
1. What makes something "iterable" in Python?
2. Why would you build a custom iterator instead of using a list?
3. Confidence level 1-10 for pythonic patterns?

## 📦 COMMIT
```bash
git add -A
git commit -m "✨ Week 5 Complete: Pythonic thinking"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

