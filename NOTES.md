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

### Day 6-7: Fork & Clone
```bash
git clone <url>                      # Download repository
git remote add upstream <url>        # Connect to original repo
git fetch upstream                   # Get upstream changes
git merge upstream/main              # Sync with original
```

### Week 2: Contribution Workflow
```bash
# Full contribution flow
git checkout -b feature-name         # Create feature branch
git add .                            # Stage changes
git commit -m "type: description"    # Commit with message
git push origin feature-name         # Push to your fork
# Then create PR on GitHub
```

## Key Concepts
- **Repository**: A folder tracked by Git
- **Staging Area**: Where changes wait before commit
- **Commit**: A snapshot of your code at a point in time
- **Branch**: An independent line of development
- **Remote**: A repository on GitHub (or other server)
- **Push**: Upload commits to remote
- **Merge**: Combine changes from one branch into another
- **Fork**: Your copy of someone else's repo on GitHub
- **Clone**: Download a repository to your computer
- **Upstream**: The original repository you forked from
- **Pull Request (PR)**: Request to merge your changes into original repo
