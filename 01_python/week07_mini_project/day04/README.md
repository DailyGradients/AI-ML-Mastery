# Week 7 — Day 4: Output Results

## 🎯 Today's Objective
Build clean, formatted output.

## 📘 LEARN (15-20 min)
**No new concepts.** Focus on presentation.

## 💻 BUILD (30-40 min)
Create `reporter.py` in this folder.

**Functions:**
```python
def print_summary(summary):
    """Print overall summary to console."""
    print("=" * 50)
    print("WAREHOUSE SHIFT REPORT")
    print("=" * 50)
    # Format nicely

def print_top_performers(performers):
    """Print top performers table."""
    pass

def write_report_file(data, output_path):
    """Write full report to a text file."""
    pass
```

**Also create `main.py`** that ties everything together:
```python
from loader import load_and_clean
from processor import shift_summary, top_performers, by_employee
from reporter import print_summary, print_top_performers, write_report_file

def main():
    print("Loading data...")
    rows, stats = load_and_clean("sample_data.csv")

    print("Processing...")
    summary = shift_summary(rows)
    top3 = top_performers(rows, n=3)

    print_summary(summary)
    print_top_performers(top3)
    write_report_file(summary, "report.txt")

if __name__ == "__main__":
    main()
```

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. What makes output readable vs hard to read?
2. Why separate the reporter from the processor?
3. How does this project feel compared to Week 1's calculator?

## 📦 COMMIT
```bash
git add -A
git commit -m "🏗️ Week 7 Day 4: Output and reporting"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

