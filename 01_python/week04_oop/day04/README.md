# Week 4 — Day 4: DataLoader Class

## 🎯 Today's Objective
Build a complete class that ties everything together.

## 📘 LEARN (15-20 min)
**No new concepts.** Today you combine everything.

**Concepts to review:**
- Classes, `__init__`, methods, properties
- File I/O, error handling
- Returning data in a structured way

## 💻 BUILD (30-40 min)
Create `day04_data_loader.py` in this folder.

**Build a DataLoader class:**
```python
class DataLoader:
    def __init__(self, filepath):
        self.filepath = filepath
        self.raw_data = []
        self.clean_data = []
        self.stats = {}

    def load(self):
        """Load the CSV file."""
        pass

    def clean(self):
        """Remove rows with missing values, convert types."""
        pass

    def calculate_stats(self):
        """Calculate summary stats for numeric columns."""
        pass

    def summary(self):
        """Print a summary."""
        pass

    def to_csv(self, output_path):
        """Export clean data."""
        pass
```

**Use it like this:**
```python
loader = DataLoader("sample_shifts.csv")
loader.load()
loader.clean()
loader.calculate_stats()
loader.summary()
loader.to_csv("cleaned_shifts.csv")
```

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. How did OOP make this code more organized than functions alone?
2. What would be hard about doing this without classes?
3. When might OOP make things WORSE instead of better?

## 📦 COMMIT
```bash
git add -A
git commit -m "🏗️ Week 4 Day 4: DataLoader class"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

