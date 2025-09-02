# Common git commandos
This document intends to show some of the commonly used git commands, as well as explain how it can help you when developing software.
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
