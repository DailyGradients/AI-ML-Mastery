# Week 4 — Day 3: Methods

## 🎯 Today's Objective
Understand different method types. Build a ModelResult class.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- Instance methods (take `self`)
- Class methods (`@classmethod`, take `cls`)
- Static methods (`@staticmethod`, take nothing)
- When to use each type
- Properties vs methods

**Read:**
- [Real Python: Instance, Class, and Static Methods](https://realpython.com/instance-class-and-static-methods-demystified/)

## 💻 BUILD (30-40 min)
Create `day03_model_result.py` in this folder.

**Build a ModelResult class:**
```python
class ModelResult:
    def __init__(self, model_name, predictions, actual):
        self.model_name = model_name
        self.predictions = predictions
        self.actual = actual

    @property
    def accuracy(self):
        """Calculate accuracy."""
        correct = sum(1 for p, a in zip(self.predictions, self.actual) if p == a)
        return correct / len(self.actual)

    def summary(self):
        """Print a summary."""
        print(f"Model: {self.model_name}")
        print(f"Accuracy: {self.accuracy:.2%}")

    @classmethod
    def from_file(cls, filepath):
        """Alternative constructor: load from a file."""
        # Load predictions and actual from a CSV
        pass

    @staticmethod
    def compare(result1, result2):
        """Compare two results and return the better one."""
        return result1 if result1.accuracy > result2.accuracy else result2
```

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. When would you use an instance method vs a class method vs a static method?
2. What's an "alternative constructor" and why are they useful?
3. What's the difference between a method and a property?

## 📦 COMMIT
```bash
git add -A
git commit -m "🏗️ Week 4 Day 3: Methods and ModelResult"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

