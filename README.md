# Git Command Cheat Sheet

Guide for some operational git command cheat sheet

---

## Configuration

### Git config username

```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

---

## Branch Management

### Git branch delete

```bash
git branch -d <branch-name>
git branch -D <branch-name>
```

### Git create new branch with new name

```bash
git switch -c <new-branch-name> origin/<remote-branch-name>
```

---

## Fetching & Pulling

### Git pull

```bash
git pull
```

### Git fetch all

```bash
git fetch --all
```

---

## Rebasing

### Git rebase procedure

```bash
git fetch origin
git rebase origin/your-branch-name
```

or

```bash
git pull --rebase --autostash
```

---

## Stashing

### Git stash procedure

```bash
git stash push --staged -m ""
```

---

## Reset

### Git reset (soft and hard)

```bash
git reset --soft HEAD~1
git reset --hard HEAD~1
```

---

## History & Blame

### Git log

```bash
git log -1 --date-order
```

### How to blame people

```bash
git log -1 --follow --format="%H|%ad|%an <%ae>|%s" <file_path>
git blame -w path/to/file
```
