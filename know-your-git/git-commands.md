# GIT Commands

Here’s a complete guide to GitHub commands, broken down into three levels—**basic**, **intermediate**, and **advanced**—with clear explanations to help you understand Git and GitHub better. Let's dive in!

---

## **Basics (Getting Started with Git and GitHub)**

### 1. **`git init`**: Initialize a Git repository
   - **What it does**: Sets up a new Git repository in your current directory. This is the first command you run to start tracking a project.
   - **Use it**: `git init`

### 2. **`git clone [URL]`**: Clone a repository
   - **What it does**: Downloads an existing Git repository from GitHub or any Git server onto your local machine.
   - **Use it**: `git clone https://github.com/username/repository.git`

### 3. **`git status`**: Check repository status
   - **What it does**: Shows the current state of the working directory, including files that are staged for commit, not staged, or untracked.
   - **Use it**: `git status`

### 4. **`git add [file]`**: Add files to the staging area
   - **What it does**: Stages a file for committing. Files must be staged before they can be committed to the repository.
   - **Use it**: 
     - To add one file: `git add filename`
     - To add all changes: `git add .`

### 5. **`git commit -m "message"`**: Commit your changes
   - **What it does**: Records the staged changes with a descriptive message that explains what was changed.
   - **Use it**: `git commit -m "Added feature X"`

### 6. **`git push`**: Push changes to GitHub
   - **What it does**: Uploads your local commits to a remote repository (like GitHub). 
   - **Use it**: `git push origin main`

### 7. **`git pull`**: Fetch and merge updates
   - **What it does**: Fetches changes from a remote repository and merges them into your current branch.
   - **Use it**: `git pull origin main`

### 8. **`git log`**: View commit history
   - **What it does**: Displays a log of all commits made to the current branch, with information like commit messages and IDs.
   - **Use it**: `git log`

---

## **Intermediate (Collaborating and Managing Workflow)**

### 1. **`git branch`**: Manage branches
   - **What it does**: Lists all branches in your repository. You can also create and delete branches.
   - **Use it**: 
     - List branches: `git branch`
     - Create a branch: `git branch feature-branch`
     - Delete a branch: `git branch -d feature-branch`

### 2. **`git checkout [branch]`**: Switch between branches
   - **What it does**: Switches your working directory to the specified branch. Useful when working on different features.
   - **Use it**: `git checkout feature-branch`

### 3. **`git merge [branch]`**: Merge branches
   - **What it does**: Combines changes from one branch into another. Usually used to bring feature work into the main branch.
   - **Use it**: `git merge feature-branch`

### 4. **`git fetch`**: Fetch changes from a remote repository
   - **What it does**: Downloads new commits from a remote repository but doesn’t merge them into your working branch.
   - **Use it**: `git fetch origin`

### 5. **`git remote -v`**: View remotes
   - **What it does**: Lists the remote connections (like GitHub repositories) associated with your project.
   - **Use it**: `git remote -v`

### 6. **`git stash`**: Stash changes
   - **What it does**: Temporarily stores changes you've made but haven't committed, so you can work on something else without committing unfinished work.
   - **Use it**: `git stash`
   - **Retrieve it**: `git stash apply`

### 7. **`git rebase`**: Reapply commits on top of another base
   - **What it does**: Moves or applies commits from one branch onto another. This helps keep a clean commit history.
   - **Use it**: `git rebase main`

### 8. **`git tag [tag-name]`**: Tag a specific commit
   - **What it does**: Marks a specific commit with a tag, typically used to denote a release version.
   - **Use it**: 
     - Lightweight tag: `git tag v1.0`
     - Annotated tag (with message): `git tag -a v1.0 -m "Release version 1.0"`

### 9. **`git reset [file]`**: Unstage files
   - **What it does**: Removes files from the staging area but keeps the changes in the working directory.
   - **Use it**: `git reset filename`

---

## **Advanced (Mastering Git)**

### 1. **`git cherry-pick [commit-hash]`**: Apply a specific commit
   - **What it does**: Applies the changes from a specific commit to your current branch, even if the commit is from another branch.
   - **Use it**: `git cherry-pick a1b2c3d`

### 2. **`git bisect`**: Find the commit that introduced a bug
   - **What it does**: Uses a binary search to find the commit that introduced a bug by checking out and testing various commits.
   - **Use it**: 
     - Start: `git bisect start`
     - Mark bad commit: `git bisect bad`
     - Mark good commit: `git bisect good`

### 3. **`git reflog`**: View reference logs
   - **What it does**: Tracks every action (checkout, commit, etc.) done in your repository, even those that are unreachable by `git log`.
   - **Use it**: `git reflog`

### 4. **`git clean -f`**: Remove untracked files
   - **What it does**: Deletes all untracked files from your working directory. Use this with caution!
   - **Use it**: `git clean -f`

### 5. **`git submodule`**: Manage submodules
   - **What it does**: Allows you to manage repositories inside other repositories (submodules). Useful when your project depends on another project.
   - **Use it**: 
     - Add a submodule: `git submodule add [URL]`
     - Update submodules: `git submodule update`

### 6. **`git revert [commit-hash]`**: Undo a specific commit
   - **What it does**: Reverts the changes introduced by a specific commit, creating a new commit that undoes the previous one.
   - **Use it**: `git revert a1b2c3d`

### 7. **`git reset --hard [commit-hash]`**: Reset the repository to a specific commit
   - **What it does**: Resets your working directory and index to a specific commit. **Warning**: This command will discard all changes after the reset point.
   - **Use it**: `git reset --hard a1b2c3d`

### 8. **`git blame [file]`**: Show who changed each line
   - **What it does**: Displays who last modified each line in a file. Useful for tracking down bugs or understanding the history of a file.
   - **Use it**: `git blame filename`

### 9. **`git diff [branch] [branch]`**: Compare differences between branches
   - **What it does**: Shows the differences between two branches or between a branch and your current state.
   - **Use it**: `git diff main feature-branch`

### 10. **`git archive`**: Create an archive of your project
   - **What it does**: Generates a tar or zip archive from your repository.
   - **Use it**: `git archive --format=tar main | gzip > project.tar.gz`

---

These commands cover everything from starting out with Git and GitHub to mastering advanced workflows. By following these commands and their use cases, you can effectively manage any GitHub project, collaborate with others, and maintain a clean and organized repository history.
