# Flowy Todo

A clean, purple-themed todo PWA with dark mode support.

**Live site:** https://jan85.github.io/flowy-todo/
**Repository:** https://github.com/Jan85/flowy-todo

---

## Commands Used

### Check GitHub CLI authentication
```bash
gh auth status
```

### Initialize local git repository
```bash
git init
git add todo.html index.html manifest.json sw.js icon.svg
git commit -m "Add Flowy Todo app with purple UI and dark mode support"
```

### Create GitHub repository and push
```bash
gh repo create flowy-todo --public --source=. --remote=origin --push
```

### Enable GitHub Pages
```bash
gh api repos/Jan85/flowy-todo/pages \
  --method POST \
  --field 'source[branch]=master' \
  --field 'source[path]=/'
```

### Fix remote URL (if wrong account credentials are cached)
```bash
git remote set-url origin https://github.com/Jan85/flowy-todo.git
gh auth setup-git
```

### Commit and push changes
```bash
git add <file>
git commit -m "Your message"
git push
```
