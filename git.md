# Git introduction
This document intends to show some of the commonly used git commands, as well as explain how it can help you when writing code.

# Most common commands and what they do
1. `git config` - Configures your git, so that you can specify username and email linked to your commits.
2. `git init` - Allows you to initialize a git repository on your local machine.
3. `git status` - Tells you what situation stage you're in within git. Really helpful when beginning to learn git.
4. `git clone <url to remote repository>` - Clones a remote repository's source code to a local working copy on your machine. I.e it downloads a copy of the source code files on the remote repository to your machine.
5. `git pull` - Fetches and integrates new changes from the remote repository into your working copy locally. 
6. `git add` - Add all or specific files that has been changed to the staging index.
7. `git commit -m "description"` - Saves a commit of new changes (the ones you have added with git add) with a log message and commit id locally.
8. `git push` - Pushes the local repository to the remote repository. The commit that's saved locally gets integrated in the remote repository.
9. `git checkout <branch name>` - Create a new branch or switch to an existing branch.
10. `git merge`- Used to merge multiple branches. If you have a main branch and a local branch to work on changes, you can checkout to the main branch and merge the changes from the local branch into it.
11. `git log` - Show all commits of a repository.





# git config
Before you can start using Git, you need to configure it. This command allows you to specify the username and email address that will be used with your commits.

`git config --global user.name "whatever user name you want"`

`git config --global user.email "email you created your github account with"`



1. git init




___
# git init
Git init allows you to initialize a git repository on your local machine. If you want to store it on github you can upload the project you created locally, by following the instructions when creating a new repository on github. 
Generally I prefer just to create and upload the repo manually using githubs GUI, but thats personal preference

`git init`

___
# git clone
Git clone is used to clone a git repository. It takes a URL as argument, and saves a local working copy of a remote repository's source code.
When you have cloned a repository you can push and pull changes from the remote repository to your local working copy.

`git clone git@github.com:"user name on github"/"name of repo".git`
___
# git status
Git status tells you what situation or status you find yourself in. It is helpful especially when starting to learn git, to use it in between git commands.

`git status`
___
# git pull
The contents of the remote repository are fetched and integrated into your local repository using this command. 
git pull pulls the most recent changes from the remote server into the local repository, ensuring you have the most up-to-date information from your coworkers.

`git pull`
___
# git push
git commit
git branch
git checkout
git merge
git log
git add
