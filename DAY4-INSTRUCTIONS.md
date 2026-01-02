# Day 4: Push to GitHub - Instructions

## Step 1: Create Repository on GitHub
1. Go to https://github.com/new
2. Repository name: `learning-opensource`
3. Description: "My journey learning open source contribution"
4. Keep it Public
5. **DO NOT** check "Add a README file" (we already have one)
6. Click "Create repository"

## Step 2: Connect Local Repo to GitHub
Run these commands (replace YOUR-USERNAME with your GitHub username):

```bash
# Navigate to your repo
cd /Users/junaidtt/Learning/opensource/learning-opensource

# Add GitHub as remote origin
git remote add origin https://github.com/YOUR-USERNAME/learning-opensource.git

# Verify remote was added
git remote -v

# Push your code to GitHub
git push -u origin main
```

## Step 3: Authentication
When prompted for credentials:
- Username: Your GitHub username
- Password: Use a Personal Access Token (PAT), NOT your password

### How to Create a PAT:
1. GitHub → Settings → Developer settings
2. Personal access tokens → Tokens (classic)
3. Generate new token (classic)
4. Give it a name like "git-cli"
5. Select scopes: `repo` (full control)
6. Generate and copy the token
7. Use this token as your password

## Step 4: Verify
Refresh your GitHub repository page - your files should appear!

## Step 5: Make Another Commit and Push
```bash
# Edit README to mark Day 4 complete
# Then:
git add README.md
git commit -m "Mark Day 4 as complete"
git push
```
