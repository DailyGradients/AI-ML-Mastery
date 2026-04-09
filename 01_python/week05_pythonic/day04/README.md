# Week 5 — Day 4: Rewrite Old Code

## 🎯 Today's Objective
Apply Pythonic patterns to your existing work.

## 📘 LEARN (15-20 min)
**No new concepts.** Today you apply everything you've learned.

## 💻 BUILD (30-40 min)
**Task:** Take 3 scripts from Weeks 1-4 and rewrite them in Pythonic style.

Create `refactored/` folder with before/after versions.

**Things to look for:**
- Replace `range(len())` with `enumerate()`
- Replace build-up loops with comprehensions
- Use `zip()` where you were accessing multiple lists
- Consider generators for large data
- Use `dict.get()` instead of `if key in dict`

**Document what you changed and why** in a `changes.md` file.

## ✍🏽 EXPLAIN (10-15 min)
Create `reflection.md` and answer:
1. Which pythonic patterns felt most natural?
2. Which took the most getting used to?
3. Did any of your refactors make the code LESS readable? Why?

## 📦 COMMIT
```bash
git add -A
git commit -m "✨ Week 5 Day 4: Pythonic refactoring"
git push origin main
```

## ✅ Done When
- [ ] Code written and runs without errors
- [ ] Reflection completed
- [ ] Committed and pushed to GitHub

