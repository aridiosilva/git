# Git -  Git Help 

## Book Pro Git
Book 2nd Edition (2014) - The entire Pro Git book, written by Scott Chacon and Ben Straub and published by Apress, is available here. All content is licensed under the Creative Commons Attribution Non Commercial Share Alike 3.0 license. Print versions of the book are available on Amazon.com.

- [downnload eBook](https://github.com/progit/progit2-pt-br/releases/download/2.1.28/progit_v2.1.28.pdf)
- [link Interne4t Book Pro Git](https://git-scm.com/book/pt-br/v2)
- [Basics of Getting a Git Repository)(https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository)

## EGIT User Guide for ECLIPSE IDE 2020-12

- [USer Guide of Git for usewith ECLIPSE IDE](https://github.com/aridiosilva/gamificacao/blob/master/Gamificacao/help/EGit%20User%20Guide%20-%20Git%20for%20ECLIPSE%20IDE%202020-12%20in%2020-DEC-2020.pdf)

## What is a git branch?

A branch represents an independent line of development. ... The git branch command lets you create, list, rename, and delete branches. It doesn't let you switch between branches or put a forked history back together again. For this reason, git branch is tightly integrated with the git checkout and git merge commands.

## What is a master branch?

The default branch name in Git is master . As you start making commits, you're given a master branch that points to the last commit you made. Every time you commit, the master branch pointer moves forward automatically. Note. The “master” branch in Git is not a special branch.

## What is a local branch?

A local branch is a branch that only you (the local user) can see. It exists only on your local machine. ... A local tracking branch is a local branch that is tracking another branch. This is so that you can push/pull commits to/from the other branch. Local tracking branches in most cases track a remote tracking branch.

## What is difference between push and commit in git?

Git commit basically “records changes to the local repository” while git push “updates remote refs along with associated objects”. So the first one is used in connection with your local repository, while the latter one is used to interact with a remote repository.

## What is the difference between git checkout and git switch?

Well, according to the documentation you link to, its sole purpose is to split and clarify the two different uses of git checkout : git switch can now be used to change branches, as git checkout <branchname> does. git restore can be used to reset files to certain revisions, as git checkout --<path_to_file> does.
  
## Why use a develop branch?

A develop branch matters more if your process to release is complex and you need to have serious release-candidates. ... In that case it may make more sense to isolate a "release candidate" in a non-master branch (such as "develop"). That allows your team running those tests to have a branch to merge features into.

## Why do we need release branch?

They do add commits to the "release" branch to fix any problems which are found during final testing, polish up rough spots, etc. So creating the "release" branch marks the "feature freeze" point -- where they decide that only the features they have already developed are going to make it into the next public release.

## What is Git branching strategy?

Git branching strategies allow a code base to evolve organically in a coherent way. A branching strategy is a convention, or a set of rules, that describes when branches are created, naming guidelines for branches, what use branches should have, and so on.

## Why is Git branching important?

Branching allows each developer to branch out from the original code base and isolate their work from others. It also helps Git to easily merge versions later on.

## What is the best practice for branching in agile?

These are the conventions to create and merge branches in the system:

- Feature branches: Branch off from develop. Merge back into develop.
- Release branches: Branch off from develop. Merge back into develop AND master.
- Hotfix branches: Branch off from master. Merge back into develop AND master.

## How do you choose a branching strategy?

Whatever branching strategy you choose I think you should:

- Use Pull Requests. ...
- Build all branches on your Continuous Integration server. ...
- Have multiple test environments and make it easy for testers to deploy the feature branches there. ...
- Know exactly what you've deployed with Git, TeamCity and Octopus.

## What is branching strategy in DevOps?

Branching is a technique that makes a copy of the source code to create two versions that are developed separately. ... There are various forms of branching. Therefore, a DevOps team must make a choice. This choice is also called the branching strategy

## Push Command

what is a push command?  

- The git push command is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repo. It's the counterpart to git fetch , but whereas fetching imports commits to local branches, pushing exports commits to remote branches.
- e git push command is used to transfer or push the commit, which is made on a local branch in your computer to a remote repository like GitHub. The command used for pushing to GitHub is:  git push 'remote_name' 'branch_name'

In this tutorial, you'll be looking two different ways to PUSH to GitHub.

## What is merge strategy?

Git Merge Strategies. A merge happens when combining two branches. ... Git has several different methods to find a base commit, these methods are called "merge strategies". Once Git finds a common base commit it will create a new "merge commit" that combines the changes of the specified merge commits.

 What is code branching and merging?

Code branching and merging is how developers work on changes and merge them back into the mainline. Every version control system has its own approach to code branching and merging. ... And as codebases, projects, and teams grow, so do potential issues around code branching.

## How do I push to main branch GitHub?

- Check your branch
- Create and checkout to a new branch from your current commit: git checkout -b [branchname]
- Then, push the new branch up to the remote: git push -u origin [branchname]

## Setting up a repository  

This tutorial provides an overview of how to set up a repository (repo) under Git version control. This resource will walk you through initializing a Git repository for a new or existing project. Included below are workflow examples of repositories both created locally and cloned from remote repositories. This guide assumes a basic familiarity with a command-line interface.

- git init 
- git clone git 
- config

[Setting up a repository](https://www.atlassian.com/git/tutorials/setting-up-a-repository)

## Learn Git with Bitbucket Cloud

Create a Git repository Copy your Git repository and add files Pull changes from your Git repository on Bitbucket Cloud Use a Git branch to merge a file

[Learn Git with Bitbucket Cloud](https://www.atlassian.com/git/tutorials/learn-git-with-bitbucket-cloud)
