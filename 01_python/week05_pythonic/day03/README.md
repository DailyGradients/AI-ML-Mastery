# Week 5 — Day 3: Generators

## 🎯 Today's Objective
Process data lazily. Understand memory efficiency.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `yield` keyword
- Generator functions
- Generator expressions: `(x*2 for x in nums)`
- Lazy evaluation (one value at a time)
- Why generators matter for large datasets

**Read:**
- [Real Python: Python Generators](https://realpython.com/introduction-to-python-generators/)

## 💻 BUILD (30-40 min)
Create `day03_generators.py` in this folder.

**Task 1: Basic generator**
```python
def count_up_to(n):
    count = 1
    while count <= n:
        yield count
        count += 1

for num in count_up_to(5):
    print(num)
```

**Task 2: File reader generator**
Create a generator that reads a CSV file line by line WITHOUT loading it all into memory:
```python
def read_shifts_lazily(filepath):
    with open(filepath) as f:
        header = f.readline().strip().split(",")
        for line in f:
            values = line.strip().split(",")
            yield dict(zip(header, values))

# Use it
for shift in read_shifts_lazily("sample_shifts.csv"):
    print(shift)
```

**Task 3: Compare memory**
```python
# Memory-heavy
big_list = [x*2 for x in range(1_000_000)]  # creates 1M items in memory

# Memory-light
big_gen = (x*2 for x in range(1_000_000))   # creates nothing until needed
```

Use `sys.getsizeof()` to compare.

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. What's the difference between `return` and `yield`?
2. Why are generators important for ML with large datasets?
3. What's the tradeoff of lazy evaluation?

## 📦 COMMIT
```bash
git add -A
git commit -m "✨ Week 5 Day 3: Generators and lazy evaluation"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

