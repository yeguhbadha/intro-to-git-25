# Learn Git Basics 🚀

Welcome to the Git Basics Workshop! This repository contains exercises to help you learn essential Git commands.

## Workshop Prerequisites
- Git installed on your computer
- A GitHub account
- A text editor

## Getting Started

1. Fork this repository by clicking the "Fork" button at the top right of this page
2. Clone your forked repository:
```bash
git clone https://github.com/YOUR-USERNAME/git-workshop
cd git-workshop
```

## Exercises

### Exercise 1: Making Your First Commit
1. Create a new file called `introduction.txt`
2. Add your name and one fun fact about yourself
3. Stage the file:
```bash
git add introduction.txt
```
4. Commit the change:
```bash
git status  # Check what's staged
git commit -m "Add personal introduction"
```

### Exercise 2: Branching Out
1. Create and switch to a new branch:
```bash
git checkout -b feature/add-hobby
```
2. Create a file called `hobbies.txt` and list your hobbies
3. Stage and commit your changes
4. Switch back to main:
```bash
git checkout main
```

### Exercise 3: Merging Changes
1. Merge your feature branch into main:
```bash
git merge feature/add-hobby
```
2. Resolve any conflicts if they occur

### Exercise 4: Collaboration
1. Create a new branch called `feature/favorite-foods`
2. Add a file `favorite-foods.txt` with your top 3 favorite foods
3. Push your branch to GitHub:
```bash
git push origin feature/favorite-foods
```
4. Create a Pull Request on GitHub

### Exercise 5: Pulling Updates
1. Pull the latest changes from the main branch:
```bash
git checkout main
git pull origin main
```

## Common Git Commands Reference

```bash
# Repository Setup
git clone <url>          # Clone a repository
git init                 # Initialize a new repository

# Basic Commands
git status              # Check repository status
git add <file>          # Stage changes
git commit -m "message" # Commit changes
git push                # Push changes to remote
git pull                # Pull changes from remote

# Branching
git branch              # List branches
git checkout <branch>   # Switch branches
git checkout -b <name>  # Create and switch to new branch
git merge <branch>      # Merge branches

# History
git log                 # View commit history
git diff                # View changes
```

## Troubleshooting Tips
- If you make a mistake in your last commit message:
  ```bash
  git commit --amend -m "New message"
  ```
- If you need to undo staged changes:
  ```bash
  git reset HEAD <file>
  ```
- If you need to discard local changes:
  ```bash
  git checkout -- <file>
  ```

## Extra Challenges
1. Try creating multiple branches and merging them
2. Practice resolving merge conflicts
3. Experiment with `git revert` to undo commits
4. Create a `.gitignore` file and test it

## Need Help?
If you get stuck, try these steps:
1. Check `git status` to see what's happening
2. Look at the error message carefully
3. Ask a workshop mentor for help
4. Google the error message (a very real developer skill!)
