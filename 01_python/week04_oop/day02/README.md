# Week 4 — Day 2: __init__ Deep Dive

## 🎯 Today's Objective
Master the constructor. Build a Dataset class.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `__init__` is called when you create an object
- Setting initial state
- Default parameter values in `__init__`
- Validation in constructors
- Type hints (`def __init__(self, name: str, age: int):`)

**Read:**
- [Real Python: Python Class Constructors](https://realpython.com/python-class-constructor/)

## 💻 BUILD (30-40 min)
Create `day02_dataset.py` in this folder.

**Build a Dataset class that loads and stores CSV data:**
```python
class Dataset:
    def __init__(self, filepath, delimiter=","):
        self.filepath = filepath
        self.delimiter = delimiter
        self.rows = []
        self.columns = []
        self._load()  # private method

    def _load(self):
        """Load the CSV file."""
        with open(self.filepath) as f:
            # Read the first line as columns
            # Read the rest as rows (as dicts)
            pass

    @property
    def shape(self):
        """Return (num_rows, num_cols)."""
        return (len(self.rows), len(self.columns))

    def __repr__(self):
        return f"Dataset({self.filepath}, shape={self.shape})"
```

**Test it with your sample_shifts.csv from Week 3.**

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. What's the purpose of `__init__`?
2. Why use `_load` with an underscore? (Hint: Python convention)
3. What does `@property` do?
4. What's `__repr__` for?

## 📦 COMMIT
```bash
git add -A
git commit -m "🏗️ Week 4 Day 2: __init__ and Dataset class"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

