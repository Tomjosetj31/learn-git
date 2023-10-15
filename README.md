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