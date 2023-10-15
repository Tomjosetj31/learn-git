# Common Git Commands I normally use

Git is a popular version control system used by developers to manage and track changes in their code repositories. Here are some common Git commands you'll frequently use during software development.

## Basic Configuration

1. **Set Your Name and Email:**
   Configure your identity for Git, which is used for tracking commits.
   ```
   git config --global user.name "Your Name"
   git config --global user.email "your@email.com"
   ```
2. Add new SSH key to your GitHub account:
   ```
   ssh-keygen -t rsa -b 4096 -C "your@email.com"
   ```
   Copy the public key to your clipboard, go to your GitHub account settings, click on SSH and GPG keys, click on New SSH key, paste the key and click on Add SSH key.

## Development

1. **Initialize a Repository:**
   Create a new Git repository in the current directory.

   ```
   git init
   ```

2. **Clone a Repository:**
   Clone a repository from GitHub to your local machine.
   ```
   git clone <repository_url>
   ```
3. **Create a Branch:**
   Create a new branch and switch to it.
   ```
   git checkout -b <branch_name>
   ```
   Create a new branch.
   ```
   git branch <branch_name>
   ```
   Switch to a branch.
   ```
   git checkout <branch_name>
   ```
   Get a list of all branches.
   ```
   git branch
   ```
   Delete a branch.
   ```
   git branch -d <branch_name>
   ```
   Change branch name.
   ```
   git branch -m <new_branch_name>
   ```
   or
   ```
   git branch -m <old_branch_name> <new_branch_name>
   ```
4. **Commit Changes:**
   Check the status of the repository.
   ```
   git status
   ```
   Add all files to staging area.
   ```
   git add <file1> <file2>
   ```
   or
   ```
   git add .
   ```
   Commit changes to the local repository.
   ```
   git commit -m "commit message"
   ```
   Commit changes to the local repository and add all files to staging area.
   ```
   git commit -am "commit message"
   ```
   View commit history.
   ```
   git log
   ```
   View commit history with a graph.
   ```
   git log --graph --oneline --decorate --all
   ```
5. **Synchronizing with Remote**
   Pull changes from remote repository(fetch and integrate changes from remote repo).
   ```
   git pull
   ```
   Fetch from Remote.
   ```
   git fetch
   ```
   Push changes to remote repository.
   ```
   git push
   ```
   Push new branch to remote repository.
   ```
    git push --set-upstream origin <branch_name>
   ```
   Merge changes from another branch.
   ```
   git merge <branch_name>
   ```
6. **Miscellaneous**
   Stash changes(temporarily save your uncommitted changes).
   ```
   git stash
   ```
   List all stashes.
   ```
   git stash list
   ```
   Apply a stash.
   ```
   git stash apply
   ```
   Apply stash by refrence.
   ```
   git stash apply stash@{number}
   ```
   Delete a stash.
   ```
   git stash drop
   ```
   Delete a stash by refrence.
   ```
    git stash drop stash@{number}
   ```
   Delete all stashes.
   ```
   git stash clear
   ```
   Get the difference between two branches.
   ```
    git diff <branch1> <branch2>
   ```
   Get the difference between two commits.
   ```
   git diff <commit1 id> <commit2 id>
   ```
   Remove all untracked files and directories.
   ```
   git clean -f -d
   ```
   Remove an untracked file without deleting it.
   ```
   git rm --cached <file_name>
   ```
