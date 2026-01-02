# Learning Notes

## Git Commands Learned

### Day 2: Setup
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git --version
```

### Day 3: First Repository
```bash
git init              # Initialize repository
git status            # Check current state
git add <file>        # Stage a file
git add .             # Stage all files
git commit -m "msg"   # Commit with message
git log               # View commit history
git log --oneline     # Compact history
```

### Day 4: Remote & Push
```bash
git remote add origin <url>  # Connect to GitHub
git remote -v                # Verify remotes
git push -u origin main      # Push to GitHub
git push                     # Push subsequent changes
```

### Day 5: Branching
```bash
git branch                   # List branches
git checkout -b <name>       # Create & switch branch
git checkout <name>          # Switch to branch
git merge <branch>           # Merge branch into current
git branch -d <name>         # Delete local branch
```

## Key Concepts
- **Repository**: A folder tracked by Git
- **Staging Area**: Where changes wait before commit
- **Commit**: A snapshot of your code at a point in time
- **Branch**: An independent line of development
- **Remote**: A repository on GitHub (or other server)
- **Push**: Upload commits to remote
- **Merge**: Combine changes from one branch into another
