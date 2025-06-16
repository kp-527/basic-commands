# 1. Initial Setup
- git init
> Initializes a new local - git repository.
- git clone <repo_url>
> Clones an existing remote repository into a new directory.

# 2. Configuration
- git config --global user.name "Your Name"
> Sets your name for commits globally.
- git config --global user.email "you@example.com"
> Sets your email for commits globally.
- git config --list
> Displays current - git configuration settings.

# 3. Staging and Committing
- git status
> Shows the working directory and staging area status.
- git add <file>
> Stages a specific file for commit.
- git add .
> Stages all changes in the current directory.
- git reset <file>
> Unstages a file while keeping the changes.
- git commit -m "message"
> Commits staged changes with a message.
- git commit -am "message"
> Stages and commits tracked file changes (not new files).

# 4. Branching and Remote Setup
- git branch
> Lists all local branches.
- git branch <branch_name>
> Creates a new branch.
- git checkout <branch_name>
> Switches to the specified branch.
- git checkout -b <branch_name>
> Creates and switches to a new branch.
- git switch <branch_name>
> Switches to a branch (modern alternative to checkout).
- git switch -c <branch_name>
> Creates and switches to a new branch.
- git remote add origin <url>
> Adds a remote repository named 'origin'.
- git remote -v
> Lists configured remote repositories.

# 5. Pushing and Pulling
- git push -u origin main
> Pushes the 'main' branch to remote and sets upstream.
- git push
> Pushes local commits to the remote repository.
- git pull
> Fetches and merges changes from the remote branch.
- git fetch
> Downloads objects and refs from another repository.

# 6. Viewing and Comparing
- git log
> Displays the commit history.
- git diff
> Shows changes between working directory and index.
- git diff --staged
> Shows differences between staged changes and the last commit.

# 7. Undoing and Reverting
- git reset --soft <commit>
> Moves HEAD to a previous commit (keeps changes staged).
- git reset --hard <commit>
> Resets index and working directory (discards changes).
- git revert <commit>
> Creates a new commit that reverses the changes.

# 8. Tagging
- git tag
> Lists all tags in the repository.
- git tag <tag_name>
> Creates a lightweight tag.
- git tag -a <tag_name> -m "message"
> Creates an annotated tag with a message.
- git push origin <tag_name>
> Pushes the specified tag to remote.

# 9. Cleanup and Maintenance
- git clean -n
> Shows untracked files that would be deleted.
- git clean -f
> Deletes untracked files.
- git gc
> Performs garbage collection and repository optimization.

# 10. Collaboration Commands
- git merge <branch>
> Merges another branch into the current branch.
- git rebase <branch>
> Reapplies commits on top of another base tip.
- git stash
> Temporarily saves changes for a clean working directory.
- git stash apply
> Applies the most recent stash.
