---
layout: page
title: Common Commands
permalink: /resources/common-commands/
nav_order: 2
parent: Resources
---

# Cheatsheat of Common Commands

Text following "#" are comments.

Text following "$" indicate commands to be used in a command line (e.g., the command prompt on Windows or terminal on macOS).

Text within "<>" indicate values for you to update (do not include the "<" and ">" characters).

## Git

```shell
# clone a repo from GitHub
$ pwd                       # print working directory to make sure you are in the correct directory
$ git clone <repo-link>     # clone the repo to your local machine
$ cd <repo-name>  # change directory into the repo
$ git status                # check that your working directory is clean

# checkout a feature branch
$ git checkout -b <branch-name>

# stage and commit changes
$ git status  # see what has been modified
$ git add <path-to-modified-file>
$ git status  # make sure this shows what you expect before committing
$ git commit -m "<useful commit message>"

# push changes to GitHub and created a PR for review
$ git push --set-upstream origin <branch-name>  # push feature branch to GitHub
# add your partner as a collaborator to your repo so they can review your code
#   1. navigate to your GitHub lab repo in a web browser
#   2. click "Settings" (upper left)
#   3. click "Collaborators & teams" (left)
#   4. enter your partner's GitHub username in "Search by username, full name or email address"
#   5. click "Add collaborator"
# create a PR to have your partner review your code before merging into your main branch
#   1. navigate to your GitHub lab repo in a web browser
#   2. click "Pull requests" (top row)
#   3. click "Compare & pull request" in the "Code" tab or "New pull request" tab
#   4. update the pull request title and leave a comment if needed
#   5. click "Reviewers" and add your partner as the reviewer
#   6. click "Create pull request"

# merge and clean up branches
# merge your feature branch into your main branch through GitHub
# delete the feature branch (on GitHub) after it is successfully merged
$ git checkout main  # check out your main branch to update it
$ git pull origin main  # pull changes from GitHub, addressing any conflicts that may arise
$ git branch -d <branch-name>  # delete your local feature branch
```

## Jupyter

```shell
# open a jupyter notebook
$ pwd               # print working directory to make sure you are in the correct directory
$ jupyter notebook  # open jupyter in your web browser then click the `.ipynb` file you want to open
```

## Conda commands

```shell
$ conda activate <env-name>           # activate an environment (macOS or Anaconda prompt)
$ source activate <env-name>          # activate an environment (Windows)
$ conda info --envs                   # show available and current environments
$ conda list                          # show packages in current environment
$ conda env export --from-history > environment.yml  # export your current environment
$ conda env remove --name <env-name>  # remove an environment
```

## Unix commands

```shell
$ ls                # list items within your current working directory (macOS, Git BASH)
$ dir               # list items within your current working directory (Anaconda Prompt)
$ cd <path>         # change to a directory
$ cd ..             # change to the parent directory
$ mkdir <dir-name>  # make a directory
$ cp <original-file-path> <new-file-path>  # copy a file
$ rm <file-path>    # remove a file
$ open <file-name>  # open a file (using default editor)
$ atom <file-name>  # open a file (using Atom)
$ alias shortcut="longer command I don't want to type out everytime I use it"
                    # aliases can be made permanant by saving this line to the ~/.bashrc file
```
