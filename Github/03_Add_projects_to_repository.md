## Initial add to a repository
To add your project to a GitHub repository, you can follow these steps:

git init
git remote add origin https://github.com/your-username/your-repo-name.git
git branch -M main
git add .
git commit -m "Initial commit"
git push -u origin main

*Explanation of each command:*
1. `git init`: Initializes a new Git repository in your project directory. This creates a hidden `.git` folder that tracks all changes to your files.
2. `git remote add origin https://github.com/your-username/your-repo-name.git`: Adds a remote repository named "origin" with the specified URL.
3. `git branch -M main`: Renames the default branch from "master" to "main".
4. `git add .`: Stages all changes in the working directory for the next commit.
5. `git commit -m "Initial commit"`: Commits the staged changes with a descriptive message.
6. `git push -u origin main`: Pushes the committed changes to the remote repository and sets the upstream branch.

## Add project to existing repository
If you already have a GitHub repository and want to add your project to it, you can follow these steps:
git pull origin main
git add .
git commit -m "Add existing project"
git push -u origin main

*Explanation of each command:*
1. `git pull origin main`: Fetches the latest changes from the remote repository and merges them into your local branch. This ensures that your local repository is up to date with the remote before you add your project.
2. `git add .`: Stages all changes in the working directory for the next commit.
3. `git commit -m "Add existing project"`: Commits the staged changes with  a descriptive message.
4. `git push -u origin main`: Pushes the committed changes to the remote repository and sets the upstream branch.   

## Check status of the repository
To check the status of your repository, you can use the following command:  
git fetch origin
git status

*Explanation of each command:*
1. `git fetch origin`: Fetches the latest changes from the remote repository without merging them into your local branch. This allows you to see if there are any new commits or changes in the remote repository.
2. `git status`: Displays the current status of your working directory and staging area. It shows which files are modified, staged for commit, or untracked. It also indicates if your local branch is ahead, behind, or has diverged from the remote branch.

## Difference between git push -u origin main, git push origin main, git push origin main --force and git push

| Command                        | Simple Meaning                                                         | When to Use                                          |
| ------------------------------ | ---------------------------------------------------------------------- | ---------------------------------------------------- |
| `git push -u origin main`      | Pushes `main` branch and connects it with remote branch for future use | First time pushing a new branch to remote            |
| `git push origin main`         | Pushes `main` branch to GitHub/remote                                  | Normal push when upstream is not set                 |
| `git push origin main --force` | Forcefully pushes and overwrites remote history                        | When commit history was changed (rebase/reset/amend) |
| `git push`                     | Pushes current branch using saved remote settings                      | Daily use after upstream is configured               |


### Common Workflow

First time: git push -u origin main

After that (regular use): git push

Only if history changed: git push --force


