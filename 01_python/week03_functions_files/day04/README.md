# Week 3 — Day 4: Logging

## 🎯 Today's Objective
Replace print() with proper logging. Learn why this matters in production.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `logging` module vs `print()`
- Log levels: DEBUG, INFO, WARNING, ERROR, CRITICAL
- `logging.basicConfig()`
- Log formatting with timestamps
- Logging to both console and file

**Read:**
- [Real Python: Python Logging](https://realpython.com/python-logging/)

## 💻 BUILD (30-40 min)
Create `day04_logging.py` in this folder.

**Task:** Take your data loader from Day 3 and add proper logging.

```python
import logging

# Set up logging to both console and file
logging.basicConfig(
    level=logging.INFO,
    format='%(asctime)s - %(levelname)s - %(message)s',
    handlers=[
        logging.FileHandler('shift_processor.log'),
        logging.StreamHandler()
    ]
)

logger = logging.getLogger(__name__)

def load_shifts(filepath):
    logger.info(f"Starting to load {filepath}")
    try:
        # Load the CSV
        logger.info(f"Successfully loaded {len(rows)} rows")
        return rows
    except FileNotFoundError:
        logger.error(f"File not found: {filepath}")
        return []
    except Exception as e:
        logger.error(f"Unexpected error: {e}")
        return []
```

Demonstrate logging at all 5 levels (DEBUG, INFO, WARNING, ERROR, CRITICAL).

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. Why is `logging` better than `print()` for production code?
2. What are the 5 log levels and when would you use each?
3. Why is it useful to log to a file AND the console?
4. What's one thing you can do with logging that you can't do with print?

## 📦 COMMIT
```bash
git add -A
git commit -m "🔧 Week 3 Day 4: Logging"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

