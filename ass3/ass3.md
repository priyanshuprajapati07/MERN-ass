# Assignment 3 – Terminal Navigation Practice Sheet

## Objective
To learn basic terminal commands for navigating directories, creating files and folders, copying, renaming, deleting files, and opening projects in Visual Studio Code.

## Command Reference

| # | Task | macOS / Linux / Git Bash | Windows PowerShell |
|---|---|---|---|
| 1 | Show current folder | `pwd` | `pwd` |
| 2 | List files | `ls` | `ls` |
| 3 | Show hidden files and details | `ls -la` | `ls -Force` |
| 4 | Create a folder | `mkdir practice` | `mkdir practice` |
| 5 | Enter a folder | `cd practice` | `cd practice` |
| 6 | Create an empty file | `touch index.html` | `New-Item index.html -ItemType File` |
| 7 | Create nested folders | `mkdir -p css/images` | `mkdir css/images` |
| 8 | Go up one level | `cd ..` | `cd ..` |
| 9 | Go to home directory | `cd ~` | `cd ~` |
| 10 | Copy a file | `cp index.html backup.html` | `Copy-Item index.html backup.html` |
| 11 | Rename or move a file | `mv backup.html old.html` | `Rename-Item backup.html old.html` |
| 12 | Delete a file | `rm old.html` | `Remove-Item old.html` |
| 13 | Delete a folder and its contents | `rm -r css` | `Remove-Item css -Recurse` |
| 14 | Display file contents | `cat index.html` | `Get-Content index.html` |
| 15 | Clear the terminal | `clear` | `cls` |
| 16 | Open the current folder in VS Code | `code .` | `code .` |

## Practice Exercise

### Tasks

1. Create a `website` folder containing `index.html`, `css/style.css`, and an `images` folder.
2. Enter the `css` directory and return to `website` using `cd ..`.
3. List all files and directories recursively.
4. Rename `index.html` to `home.html`, then rename it back to `index.html`.
5. Open the project folder in Visual Studio Code.

### Commands Used — Windows PowerShell

Run the following commands one by one, starting from your home directory.

```powershell
cd ~
mkdir website
mkdir website/css
mkdir website/images
New-Item website/index.html -ItemType File
New-Item website/css/style.css -ItemType File
cd website/css
cd ..
Get-ChildItem -Recurse
Rename-Item index.html home.html
Rename-Item home.html index.html
code .
```

## Expected Folder Structure

```text
website/
├── index.html
├── css/
│   └── style.css
└── images/
```

## Conclusion

I practised essential terminal commands for directory navigation, file and folder creation, copying, renaming, deleting, and listing files. These commands help me manage web development projects efficiently and work comfortably with Git and Visual Studio Code.