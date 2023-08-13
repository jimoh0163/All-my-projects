
 # GIT PROJECT
I will be demonstrating how to efficiently initialized a repository and make commits work with Branches, collaboration, and Remote repositories, and Tagging track change, highlighting the significance of git in modern software development workflows


## INITIALIZING A REPOSITORY AND MAKING COMMITS

let's start by introducing GIT

## WHAT IS GIT

Git is a distributed version control system that tracks changes in any set of computer files, usually used for coordinating work among programmers who are collaboratively developing source code during software development. Its goals include speed, data integrity, and support for distributed, non-linear workflows (thousands of parallel branches running on different computers).

## INITIALIZING GIT REPOSITORY

 Before initializing a git repository you must have installed git on your computer 
 
To initialize a git repo follow the steps

-Open a terminal on your computer, eg git bash,

-On your terminal create your working folder or directory eg Dev0ps folder using the command 

**`mkdir Dev0ps`**

-Change or move into your working folder or directory eg Dev0ps folder using

**`cd Dev0ps`**

-while you are inside the folder, run git init command

**`git init`**


![Capture1](https://github.com/jimoh0163/All-my-projects/assets/140582025/4db98247-079b-44f6-a615-bd8e519f02bb)


# Making your first Commit

Before making our first commit let's try to understand what a commit is in git.

Commit is more or less saving the changes you made to your files.

Changes can be adding, modifying, or deleting files or text.

When you make a commit, git takes a snapshot of the current state of your repository and saves a copy in the .git folder inside your working directory.

# Let's make our first commit by following these steps.

-inside your working directory create a file index.txt using the command touch index.txt

**`touch index.txt`**

-Write any sentence of your choice inside the text file. Afterward, save your changes

-Add your changes to git staging area using this command 

**`git add .`**

-To commit your changes to git, run the command 

**`git commit -m "initial commit`**

![Capture2](https://github.com/jimoh0163/All-my-projects/assets/140582025/66e17a6c-a549-450f-b652-527c83b23fbf)

The -m flag is used to provide a commit message. The commit message is a nice way to provide context about the commit. When writing a commit message, make it descriptive as possible. Let it explain why the commit was made

## Working with Branches

Imagine you have a notebook and you want to write different on pages of your notebook so that you do not mess up your previous note.

git branch helps you create a different copy(page) of your source code.

In your new branch you can make changes as you please. Your change is independent of what is available in the main copy

Git branch is commonly used to develop new features of your application. 

you will agree with me that the initial code is untested and such can not be added to the code base of my live application

Git branch is also an important tool for collaboration within remote teams(developers working from different locations). They can make separate branches while working on the same feature. And at the end of the day, converge their code to one branch



# Make your first git branch

To make a new branch run this command:

**`git checkout -b`**

The -b flag helps you create and change into the new branch with that said let's make our first branch following these steps

-Having made your first commit in the previous lessons

-Make a new branch by running this command 

**`git checkout -b my-new-branch`**


![Capture3](https://github.com/jimoh0163/All-my-projects/assets/140582025/494476db-6d93-48d2-a5b0-d89649c4a820)


# Listing your git branches

use the below command to list the branches on your local git repository

**`git branch`**

![Capture6](https://github.com/jimoh0163/All-my-projects/assets/140582025/7166a218-1ecf-4ddf-892d-212eeb38e92c)

## Change into an Old Branch

To change into an existing or old branch use the command below

**`git checkout (branch name)`**

![Capture7](https://github.com/jimoh0163/All-my-projects/assets/140582025/01e29185-1548-417f-adc7-11706e29d6f4)

## Merging Branch into another Branch

Let's say we have two branches A and B. And we want to add the content of branch B into A

First we change into branch A and run the git command below

**`git merge B`**


![Capturemerge](https://github.com/jimoh0163/All-my-projects/assets/140582025/4a00015c-3e3f-4d22-a142-23fc5011cbaf)

## Deleting a git branch

When a new feature is added to an application, it's often done in a feature branch. Usually this feature branch is deleted when the code must have tested and merged into a staging or dev environment depending on the branch strategy of the team.

![Capture8d](https://github.com/jimoh0163/All-my-projects/assets/140582025/1ed920eb-d495-46f5-935e-a134a0e54218)
