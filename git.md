# Git introduction
This document intends to show some of the commonly used git commands, as well as explain how it can help you when writing code.

# Most common commands and what they do
1. `git config` – Set username and email for commits.
2. `git init` – Initialize a local repository.
3. `git status` – Show current repository state.
4. `git clone <url>` – Copy a remote repository locally.
5. `git pull` – Update local copy with remote changes.
6. `git add . / git add <file>` – Stage changes.
7. `git commit -m "msg"` – Save staged changes with a message.
8. `git push` – Upload local commits to remote.
9. `git checkout <branch>` – Switch or create a branch.
10. `git merge <branch>` – Merge a branch into the current one.
11. `git log` – View commit history

# Common workflows
## Starting a new project
1. Go to github.com and log in to your account.
2. Press create new repository, and name it.
3. You can either manually upload the inital commit (a or some files) or you can initialize it in you command line.
If you want to use the command line, create a directory and store the inital files for your new project.
Move to the directory in the command line and run `git init`.
Then on github where you created the repository you need to do the 3 git commands under "…or push an existing repository from the command line".
4. Once you have made the inital commit in step 3 you should clone the repository on github, so that you get a local copy on your computer.
   Move to a directory where you want to save the project locally, and use `git clone <git@github.com:"username on github"/"repo name on github".git>`
5. Now you should have a remote repository stored on github and a clone of this repo locally on your machine. The repository on github can (and should) be shared with your collaborators, so that all of you can clone it and push and pull changes to the project.

## Working on a project
1. At this point you should have a working git repository stored on github, and cloned locally to your machine.
2. Git will track your changes to the code made locally (You could be writing new files or changing existing code in the project).
3. If you made any changes to the code that you want to be uploaded to your shared remote repository on github you should use `git add .` if you want to add all changes to every file you have made, or `git add filnavn.filtype` if you want to pick specific files.
4. Once you've added the files to the staging index (git add), you use `git commit -m "I changed xyz in file xyz"` to store the commit locally. Then finally you can use `git push` this pushes the changes onto the github source code, making the version you commited the newest version. Collaborators in the group should then remember to fetch changes by using `git pull` so that everyone is up to date

## Multiple branches
1. It is a good idea to make an additional branch locally when working on a shared project. This allows you to keep a main branch (the one on github) with the projects current source code. In addition to the main branch you can create a new one locally, so that you can experiment
