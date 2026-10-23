# Assignment 5 – GitHub Repository Link

## Objective
To create a GitHub repository, push the local project to GitHub, and share the repository link.

## Steps to Push the Project

### 1. Create a GitHub Repository

1. Open [GitHub](https://github.com/).
2. Click **New repository**.
3. Enter the repository name: `html-css-assignments`.
4. Keep the repository empty without adding a README, `.gitignore`, or license if you are pushing an existing local project.
5. Click **Create repository**.

### 2. Connect the Local Repository to GitHub

Open the terminal in your local project folder and run:

```bash
git remote add origin https://github.com/priyanshuprajapati07/html-css-assignments.git
git branch -M main
git push -u origin main
```


If the `origin` remote is already configured, check it using:

```bash
git remote -v
```

If it points to the correct repository, you do not need to add it again.

### 3. Verify the Upload

1. Refresh the GitHub repository page.
2. Confirm that the project files and `README.md` are visible.
3. Open the commit history