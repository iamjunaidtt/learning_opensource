# Week 2: Making Your First Contribution

## Day 8: The Contribution Workflow

### The Complete Flow
```
Fork → Clone → Branch → Edit → Commit → Push → Pull Request
```

### Prerequisites
Make sure you've completed Days 6-7:
- Forked first-contributions to your account
- Cloned it to your computer

### Step 1: Navigate to your clone
```bash
cd /Users/junaidtt/Learning/opensource/first-contributions
```

### Step 2: Create a new branch
```bash
# Create branch with your name
git checkout -b add-junaid-tt

# Verify you're on the new branch
git branch
```

### Step 3: Add your name to Contributors.md
Open `Contributors.md` and add your name in alphabetical order:
```markdown
- [Junaid TT](https://github.com/junaidtt)
```

### Step 4: Stage and commit
```bash
git add Contributors.md
git commit -m "Add Junaid TT to contributors list"
```

### Step 5: Push to YOUR fork
```bash
git push origin add-junaid-tt
```

---

## Day 9: Create Your First Pull Request

### On GitHub:
1. Go to your fork: `github.com/YOUR-USERNAME/first-contributions`
2. You'll see a yellow banner: "add-junaid-tt had recent pushes"
3. Click **"Compare & pull request"**

### Fill in the PR form:
**Title:** Add Junaid TT to contributors list

**Description:**
```markdown
## What does this PR do?
Adds my name to the Contributors list.

## Checklist
- [x] Added name in alphabetical order
- [x] Followed the contribution guidelines
```

4. Click **"Create pull request"**

### 🎉 Congratulations! You've submitted your first PR!

---

## Day 10: Finding Beginner-Friendly Issues

### Search Labels on GitHub
Use these search queries:

```
# Good first issues in Python
label:"good first issue" language:python is:open

# Beginner-friendly JavaScript projects
label:"beginner-friendly" language:javascript is:open

# Help wanted in any language
label:"help wanted" is:open

# First-timers only
label:"first-timers-only" is:open
```

### Websites to Find Issues
| Site | URL |
|------|-----|
| Good First Issue | https://goodfirstissue.dev |
| Up For Grabs | https://up-for-grabs.net |
| First Timers Only | https://www.firsttimersonly.com |
| Code Triage | https://www.codetriage.com |

### Practice Exercise
1. Visit https://goodfirstissue.dev
2. Filter by a language you know
3. Read 5 different issues
4. Note which ones you could potentially solve

---

## Day 11: Reading Contribution Guidelines

### Files to Look For
Every well-maintained project has these files:

| File | Purpose |
|------|---------|
| `README.md` | Project overview, setup instructions |
| `CONTRIBUTING.md` | How to contribute |
| `CODE_OF_CONDUCT.md` | Community behavior rules |
| `LICENSE` | Legal terms for using the code |
| `.github/ISSUE_TEMPLATE/` | Templates for filing issues |
| `.github/PULL_REQUEST_TEMPLATE.md` | PR template |

### What to Look For in CONTRIBUTING.md
- [ ] How to set up the development environment
- [ ] Code style guidelines
- [ ] Commit message format
- [ ] Branch naming conventions
- [ ] Testing requirements
- [ ] PR review process

### Practice Exercise
Read the CONTRIBUTING.md files from these projects:
1. https://github.com/freeCodeCamp/freeCodeCamp/blob/main/CONTRIBUTING.md
2. https://github.com/facebook/react/blob/main/CONTRIBUTING.md
3. https://github.com/microsoft/vscode/blob/main/CONTRIBUTING.md

---

## Day 12: Documentation Contributions (Easiest Start!)

### Why Start with Docs?
- Lower barrier to entry
- No complex setup needed
- Maintainers love doc improvements
- Great way to learn the codebase

### Types of Doc Contributions
1. **Fix typos** - Easy wins!
2. **Improve clarity** - Rewrite confusing sections
3. **Add examples** - Code samples help everyone
4. **Update outdated info** - Keep docs current
5. **Translate** - Help non-English speakers

### Practice Exercise
```bash
# Fork and clone any project
git clone https://github.com/YOUR-USERNAME/some-project.git
cd some-project

# Create a branch
git checkout -b fix/typo-in-readme

# Find and fix a typo in README.md or docs/
# Then commit with a clear message
git add .
git commit -m "docs: fix typo in README"

# Push and create PR
git push origin fix/typo-in-readme
```

### Good Commit Message Prefixes for Docs
```
docs: add installation instructions
docs: fix typo in API reference
docs: update outdated screenshot
docs: improve clarity of setup guide
```

---

## Days 13-14: Practice with "Good First Issue"

### Step-by-Step Process

#### 1. Find an Issue
```bash
# Search on GitHub
label:"good first issue" language:YOUR-LANGUAGE is:open
```

#### 2. Claim the Issue
Comment on the issue:
```
Hi! I'd like to work on this issue. Could you please assign it to me?
I'm a beginner contributor and this looks like a great starting point.
```

#### 3. Understand the Problem
- Read the issue description carefully
- Read any linked documentation
- Look at related code
- Ask questions if unclear

#### 4. Set Up the Project
```bash
# Fork and clone
git clone https://github.com/YOUR-USERNAME/project-name.git
cd project-name

# Read setup instructions
cat README.md
cat CONTRIBUTING.md

# Install dependencies (varies by project)
npm install          # Node.js
pip install -r requirements.txt  # Python
bundle install       # Ruby
```

#### 5. Create a Branch
```bash
# Use issue number in branch name
git checkout -b fix/issue-123-description
```

#### 6. Make Changes
- Write the code
- Follow project style guide
- Add tests if required
- Update documentation if needed

#### 7. Test Your Changes
```bash
# Run existing tests
npm test       # Node.js
pytest         # Python
go test ./...  # Go
```

#### 8. Commit and Push
```bash
git add .
git commit -m "fix: resolve issue #123 - description

- What you changed
- Why you changed it

Fixes #123"

git push origin fix/issue-123-description
```

#### 9. Create Pull Request
- Go to your fork on GitHub
- Click "Compare & pull request"
- Fill in the template
- Reference the issue: "Fixes #123"

#### 10. Respond to Feedback
- Be patient and polite
- Make requested changes
- Push updates to same branch
- Thank reviewers!

---

## Week 2 Checklist

- [ ] Day 8: Create branch and edit Contributors.md
- [ ] Day 9: Submit first Pull Request
- [ ] Day 10: Find 5 beginner-friendly issues
- [ ] Day 11: Read 3 CONTRIBUTING.md files
- [ ] Day 12: Submit a documentation PR
- [ ] Day 13-14: Work on a "good first issue"

---

## Commands Summary

```bash
# Contribution workflow
git checkout -b feature-name    # Create branch
git add .                       # Stage changes
git commit -m "type: message"   # Commit
git push origin feature-name    # Push to fork

# Sync with upstream
git fetch upstream              # Get latest changes
git checkout main               # Switch to main
git merge upstream/main         # Merge upstream
git push origin main            # Update your fork
```

## Commit Message Types
| Type | Use For |
|------|---------|
| `feat` | New feature |
| `fix` | Bug fix |
| `docs` | Documentation |
| `style` | Formatting (no code change) |
| `refactor` | Code restructure |
| `test` | Adding tests |
| `chore` | Maintenance tasks |
