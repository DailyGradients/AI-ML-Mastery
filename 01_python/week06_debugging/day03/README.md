# Week 6 — Day 3: Defensive Programming

## 🎯 Today's Objective
Handle errors gracefully with try/except.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `try` / `except` / `else` / `finally`
- Catching specific exceptions (not bare `except:`)
- Custom exception types
- When to catch vs let it crash
- EAFP vs LBYL philosophy

**Read:**
- [Real Python: Python Try/Except](https://realpython.com/python-exceptions/)

## 💻 BUILD (30-40 min)
Create `day03_defensive.py` in this folder.

**Build an error-safe data loader:**
```python
import logging

logger = logging.getLogger(__name__)

def safe_load_shifts(filepath):
    """Load shifts with comprehensive error handling."""
    try:
        with open(filepath) as f:
            # Try to parse the file
            pass
    except FileNotFoundError:
        logger.error(f"File not found: {filepath}")
        return []
    except PermissionError:
        logger.error(f"Permission denied: {filepath}")
        return []
    except UnicodeDecodeError:
        logger.error(f"Encoding error in {filepath}")
        return []
    except Exception as e:
        logger.error(f"Unexpected error: {e}")
        return []
    else:
        logger.info(f"Successfully loaded {filepath}")
        return rows
    finally:
        logger.info("Load operation complete")
```

Test it with:
- A file that exists
- A file that doesn't exist
- A file with bad data

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. When should you catch an exception vs let it crash?
2. What's the problem with `except Exception:` (too broad)?
3. What does `finally` do?
4. What does `else` do in try/except/else?

## 📦 COMMIT
```bash
git add -A
git commit -m "🐛 Week 6 Day 3: Defensive programming"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

