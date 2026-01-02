# Days 6-7: Fork & Clone Practice

## Day 6: Fork a Repository

### What is a Fork?
A fork is YOUR copy of someone else's repository on GitHub.

```
Original repo:  github.com/firstcontributions/first-contributions
                           ↓ (Fork)
Your fork:      github.com/YOUR-USERNAME/first-contributions
```

### Steps to Fork:
1. Visit: https://github.com/firstcontributions/first-contributions
2. Click "Fork" button (top-right corner)
3. Select your GitHub account
4. Wait for GitHub to create your copy

---

## Day 7: Clone Your Fork

### Clone to Your Computer
```bash
# Navigate to your projects folder
cd /Users/junaidtt/Learning/opensource

# Clone YOUR fork (not the original!)
git clone https://github.com/YOUR-USERNAME/first-contributions.git

# Enter the cloned directory
cd first-contributions

# Verify the remote
git remote -v
```

You should see:
```
origin  https://github.com/YOUR-USERNAME/first-contributions.git (fetch)
origin  https://github.com/YOUR-USERNAME/first-contributions.git (push)
```

### Add Upstream Remote
Connect to the original repo to stay updated:
```bash
git remote add upstream https://github.com/firstcontributions/first-contributions.git

# Verify both remotes
git remote -v
```

Now you'll see:
```
origin    https://github.com/YOUR-USERNAME/first-contributions.git
upstream  https://github.com/firstcontributions/first-contributions.git
```

---

## Key Concepts

| Term | Meaning |
|------|---------|
| Fork | Copy of a repo in YOUR GitHub account |
| Clone | Download a repo to your local machine |
| Origin | Your fork on GitHub |
| Upstream | The original repo you forked from |

---

## The Contribution Workflow

```
1. Fork      → Create your copy on GitHub
2. Clone     → Download to your computer
3. Branch    → Create feature branch
4. Edit      → Make your changes
5. Commit    → Save changes locally
6. Push      → Upload to YOUR fork
7. PR        → Request to merge into original
```

---

## Practice Exercise

After cloning first-contributions:
```bash
# List the files
ls -la

# Read the README
cat README.md

# Check the contribution guide
cat CONTRIBUTING.md

# See the Contributors list
head -50 Contributors.md
```

---

## Ready for Day 8?
Tomorrow you'll:
1. Create a branch
2. Add your name to Contributors.md
3. Submit your first Pull Request!
