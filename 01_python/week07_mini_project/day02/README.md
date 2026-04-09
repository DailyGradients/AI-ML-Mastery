# Week 7 — Day 2: Load & Clean Data

## 🎯 Today's Objective
Build a robust data loader that handles messy data.

## 📘 LEARN (15-20 min)
**No new concepts.** Apply what you know from Weeks 3-6.

## 💻 BUILD (30-40 min)
Create `loader.py` in this folder.

**Requirements:**
```python
import csv
import logging

def load_raw_data(filepath):
    """Load raw CSV data into a list of dicts."""
    pass

def clean_row(row):
    """Clean a single row. Return None if row should be skipped."""
    # Check for required fields
    # Convert types (int for units, float for hours, int for errors)
    # Handle missing values
    # Return None if row is too broken to fix
    pass

def load_and_clean(filepath):
    """Load and clean the entire file. Return clean rows + stats."""
    raw = load_raw_data(filepath)
    clean = []
    stats = {
        'total_rows': len(raw),
        'clean_rows': 0,
        'missing_values': 0,
        'bad_types': 0,
        'duplicates': 0
    }

    # Process each row
    # Track stats
    # Remove duplicates

    return clean, stats
```

**Test it with your messy sample data from Day 1.**

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. What was hardest about handling the messy data?
2. What decisions did you have to make about bad rows?
3. Why track stats about what you cleaned?

## 📦 COMMIT
```bash
git add -A
git commit -m "🏗️ Week 7 Day 2: Data loader and cleaner"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

