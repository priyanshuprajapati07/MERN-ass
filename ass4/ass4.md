# Assignment 4 – Repository with at Least Three Meaningful Commits

## Objective
To create a Git repository and maintain a meaningful commit history using Git commands.

## Steps Performed

### 1. Configure Git Identity

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

### 2. Initialize the Repository

```bash
mkdir html-css-assignments
cd html-css-assignments
git init
git branch -M main
```

### 3. Commit 1 – Add README

```bash
echo "# HTML & CSS Assignments" > README.md
git add README.md
git commit -m "docs: add README with project overview"
```

### 4. Commit 2 – Add Documentation Assignments

```bash
git add 01.md 02.md 03.md 04.md 05.md
git commit -m "docs: add setup and Git assignments"
```

### 5. Commit 3 – Add HTML Assignments

```bash
git add 06.html 07.html 08.html 09.html 10.html
git commit -m "feat: add HTML basics assignments"
```

*Note: The filenames above are examples. Use the actual filenames in your repository.*

## Commit History

To view the commit history, run:

```bash
git log --oneline
```

Example output:

```text
abc1234 feat: add HTML basics assignments
def5678 docs: add setup and Git assignments
ghi9012 docs: add README with project overview
```

## Good Commit Message Practices

- Use clear and meaningful commit messages.
- Use prefixes such as `feat:`, `fix:`, `docs:`, and `style:`.
- Keep each commit focused on one logical change.

## Conclusion

I learned how to initialize a Git repository, configure Git identity, stage files, create meaningful commits, and inspect the commit history using Git commands.