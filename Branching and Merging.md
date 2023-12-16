### Git Branching:
#### Creating a Branch:

```bash
# Create a new branch
git branch branch_name

# Switch to the new branch
git checkout branch_name  # (or use 'git switch' in Git version 2.23 and later)
```

or in one step:

```bash
# Create and switch to a new branch
git checkout -b branch_name  # (or use 'git switch -c' in Git version 2.23 and later)
```

#### Listing Branches:

```bash
# List all branches
git branch
```

#### Switching Between Branches:

```bash
# Switch to a different branch
git checkout existing_branch  # (or use 'git switch')
```

### Git Merging:

Merging is the process of combining changes from different branches into a single branch, often used to integrate a feature branch back into the main branch. Here's an overview of merging:

#### Merging Changes:

```bash
# Switch to the branch you want to merge into
git checkout main_branch  # (or use 'git switch')

# Merge changes from another branch into the current branch
git merge branch_name
```

#### Resolving Merge Conflicts:

Sometimes, Git may encounter conflicts if changes in different branches overlap. In such cases, manual intervention is required to resolve conflicts.

```bash
# After resolving conflicts, finalize the merge
git add conflicted_file(s)
git merge --continue
```

#### Deleting Branches:

```bash
# Delete a local branch (after it has been merged)
git branch -d branch_name

# Force delete a branch (use with caution, as it discards changes)
git branch -D branch_name
```

### Git Workflow Example:

```bash
# Start a new feature branch
git checkout -b feature_branch

# Make changes, commit, and push the feature branch
git add .
git commit -m "Implement new feature"
git push origin feature_branch

# Switch to the main branch
git checkout main

# Merge the feature branch into the main branch
git merge feature_branch

# Push the changes to the remote repository
git push origin main

# Delete the feature branch (optional)
git branch -d feature_branch
```
