# Week 3 — Day 3: File I/O

## 🎯 Today's Objective
Read and write data to files. Learn the csv module.

## 📘 LEARN (15-20 min)
**Concepts to absorb:**
- `open()` function with modes: `"r"`, `"w"`, `"a"`
- The `with` statement (context managers)
- `read()`, `readlines()`, `write()`
- The `csv` module: `csv.reader`, `csv.DictReader`, `csv.DictWriter`
- File encoding (use `utf-8`)

**Read one of these:**
- [Real Python: Reading and Writing Files](https://realpython.com/read-write-files-python/)
- [Automate the Boring Stuff Ch 9: Files](https://automatetheboringstuff.com/2e/chapter9/)

## 💻 BUILD (30-40 min)
**Step 1:** Create a sample data file `sample_shifts.csv` with this content:

```csv
date,shift_id,supervisor,headcount,units,errors
2026-04-01,SH-001,Martinez,12,487,3
2026-04-01,SH-002,Chen,13,523,1
2026-04-02,SH-003,Rodriguez,11,445,5
2026-04-02,SH-004,Martinez,14,578,2
2026-04-03,SH-005,Chen,12,492,4
```

**Step 2:** Create `day03_file_io.py` that:
- Reads the CSV file using `csv.DictReader`
- Calculates total units and average units per shift
- Filters shifts with errors > 2
- Writes a new CSV `shifts_summary.csv` with the problem shifts
- Prints a summary report to the console

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. Why do we use `with open(...) as f:` instead of just `open(...)`?
2. What's the difference between `"r"`, `"w"`, and `"a"` modes?
3. Why is `DictReader` more useful than plain `csv.reader`?
4. What encoding should you usually use?

## 📦 COMMIT
```bash
git add -A
git commit -m "🔧 Week 3 Day 3: File I/O and CSV handling"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

