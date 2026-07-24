# Git HOL 1 - GitDemo Project

## Objectives
- Learn Git commands: `git init`, `git status`, `git add`, `git commit`, `git push`, `git pull`
- Setup Git configuration
- Add a file to a source code repository

## Steps Completed

### Step 1: Git Configuration
```bash
git --version          # Verified git version 2.48.1.windows.1
git config --global user.name "[USERNAME]"
git config --global user.email "[EMAIL_ADDRESS]"
git config --list      # Verified configuration
```

### Step 2: Create GitDemo Repository
```bash
mkdir GitDemo
cd GitDemo
git init               # Initialized empty Git repository
ls -a                  # Shows hidden .git directory
```

### Step 3: Create and Track welcome.txt
```bash
echo "Welcome to Git Demo - HOL 1" > welcome.txt
cat welcome.txt        # Verified file content
git status             # Shows welcome.txt as untracked
git add welcome.txt    # Staged the file
git status             # Shows welcome.txt as "Changes to be committed"
git commit -m "Initial commit: Add welcome.txt to GitDemo repository"
git status             # Clean working tree
git log --oneline      # Shows commit history
```

### Step 4: Push to Remote (GitLab/GitHub)
```bash
# Add your remote repository URL:
git remote add origin <your-remote-repo-url>
git pull origin master
git push origin master
```

## Commit History
- `40bd688` - Initial commit: Add welcome.txt to GitDemo repository
