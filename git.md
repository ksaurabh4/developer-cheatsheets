
# Git Command Cheat Sheet

## 🔧 **Git Setup**
```bash
git config --global user.name "Your Name"          # Set your Git username
git config --global user.email "youremail@example.com"  # Set your Git email
git config --list                                  # List all Git configurations
```

## 📁 **Create a New Repository**
```bash
git init                                           # Initialize a new Git repository
git clone <repo_url>                               # Clone a remote repository
```

## 📂 **Basic Snapshotting**
```bash
git status                                         # Show status of working directory
git add <file>                                     # Stage a specific file
git add .                                          # Stage all changed files
git commit -m "Commit message"                     # Commit staged changes
git commit -am "Commit message"                    # Stage and commit all changes (tracked files)
git rm <file>                                      # Remove a file from the working directory and staging area
```

## 🔄 **Branching and Merging**
```bash
git branch                                         # List all branches
git branch <branch_name>                           # Create a new branch
git checkout <branch_name>                         # Switch to a branch
git checkout -b <new_branch_name>                  # Create and switch to a new branch
git merge <branch_name>                            # Merge a branch into the current branch
git branch -d <branch_name>                        # Delete a branch
git branch -D <branch_name>                        # Force delete a branch
```

## 🌐 **Working with Remote Repositories**
```bash
git remote -v                                      # List remote connections
git remote add <name> <url>                        # Add a new remote
git fetch <remote>                                 # Fetch changes from a remote repository
git pull <remote> <branch>                         # Fetch and merge changes from a remote branch
git push <remote> <branch>                         # Push changes to a remote branch
git push -u <remote> <branch>                      # Push changes and set upstream for tracking
git push                                           # Push changes (if upstream set)
git remote remove <name>                           # Remove a remote repository
```

## 📜 **Inspecting and Comparing**
```bash
git log                                            # Show commit logs
git log --oneline                                  # Show commit logs in a single line per commit
git log --graph --oneline --decorate               # Show log with a graph of branches
git diff                                           # Show changes in the working directory not yet staged
git diff --staged                                  # Show changes between the staging area and the last commit
git show <commit>                                  # Show changes of a specific commit
git blame <file>                                   # Show who modified each line of a file
```

## 🚑 **Undoing Changes**
```bash
git restore <file>                                 # Discard changes in the working directory
git restore --staged <file>                        # Unstage a file (keep changes in working directory)
git reset <commit>                                 # Reset to a specific commit (keep changes)
git reset --hard <commit>                          # Reset to a commit and discard all changes
git revert <commit>                                # Create a new commit that undoes the changes of a previous commit
```

## 🏷️ **Tagging**
```bash
git tag                                            # List all tags
git tag <tag_name>                                 # Create a new tag at the current commit
git tag -a <tag_name> -m "Tag message"             # Create an annotated tag
git push <remote> <tag_name>                       # Push a specific tag to the remote
git push <remote> --tags                           # Push all tags to the remote
git tag -d <tag_name>                              # Delete a local tag
git push <remote> --delete <tag_name>              # Delete a remote tag
```

## 🧹 **Cleaning Up**
```bash
git clean -f                                       # Remove untracked files from the working directory
git clean -fd                                      # Remove untracked files and directories
```

## 🔄 **Stashing Changes**
```bash
git stash                                          # Stash current changes
git stash list                                     # List all stashes
git stash apply                                    # Apply the latest stash
git stash apply stash@{n}                          # Apply a specific stash
git stash drop                                     # Drop the latest stash
git stash drop stash@{n}                           # Drop a specific stash
git stash pop                                      # Apply and remove the latest stash
```

## 🚀 **Advanced Commands**
```bash
git rebase <branch_name>                           # Rebase current branch onto another branch
git cherry-pick <commit>                           # Apply the changes from a specific commit
git reflog                                         # Show a log of changes to the local repository
```

## 🌱 **Shortcuts**
```bash
git checkout -b <branch_name>                      # Create and switch to a new branch
git commit -am "message"                           # Add all changes and commit in one step
```
