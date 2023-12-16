### 1. Initializing a Repository

```bash
# Initialize a new Git repository
git init
```

### 2. Configuring Git

```bash
# Configure user information
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### 3. Modifying, Adding, and Committing Artifacts

```bash
# Check the status of your working directory
git status

# Add changes to the staging area
git add filename

# Add all changes to the staging area
git add .

# Commit changes with a descriptive message
git commit -m "Your commit message"
```

### 4. Inspecting Git Repository

```bash
# Show changes between commits, commit details, and file changes
git log

# Show a more compact log with one line per commit
git log --oneline

# Show the status of working directory and staging area
git status

# Show differences between working directory, staging area, and the last commit
git diff

# Show differences for a specific file
git diff filename
```
