# Git introduction
This document intends to show some of the commonly used git commands, as well as explain how it can help you when writing code.

# Most common commands and what they do
1. `git config` - Configures your git, so that you can specify username and email linked to your commits.
2. `git init` - Allows you to initialize a git repository on your local machine.
3. `git status` - Tells you what situation stage you're in within git. Really helpful when beginning to learn git.
4. `git clone <url to remote repository>` - Clones a remote repository's source code to a local working copy on your machine. I.e it downloads a copy of the source code files on the remote repository to your machine.
5. `git pull` - Fetches and integrates new changes from the remote repository into your working copy locally. 
6. `git add . || git add filnavn.filtype` - Add all or specific files that has been changed to the staging index.
7. `git commit -m "description"` - Saves a commit of new changes (the ones you have added with git add) with a log message and commit id locally.
8. `git push` - Pushes the local repository to the remote repository. The commit that's saved locally gets integrated in the remote repository.
9. `git checkout <branch name>` - Create a new branch or switch to an existing branch.
10. `git merge <branch to merge with>`- Used to merge multiple branches. If you have a main branch and a local branch to work on changes, you can checkout to the main branch and merge the changes from the local branch into it.
11. `git log` - Show all commits of a repository.

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
