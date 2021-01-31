# Git and GitHub 

- Git - An open source, distributed version-control system
- GitHub - A platform for hosting and collaborating on Git repositories

![all repos](https://github.com/aridiosilva/git/blob/main/areas_overview_of_git_project.png)


![the phases of VSC process](https://github.com/aridiosilva/git/blob/main/Tracked%20and%20Untracked%20files%20in%20GIT.jpg)

### Figure - A linear view of progressive-stability branching

![A linear view of progressive-stability branching](https://github.com/aridiosilva/git/blob/main/lr-branches-1.png)

### Figure - A “silo” view of progressive-stability branching

![A “silo” view of progressive-stability branching](https://github.com/aridiosilva/git/blob/main/lr-branches-2.png)

### Figure -  Multiple topic branches

![Multiple topic branches](https://github.com/aridiosilva/git/blob/main/topic-branches-1.png)

### Figure - History after merging dumbidea and iss91v2

![History after merging dumbidea and iss91v2](https://github.com/aridiosilva/git/blob/main/topic-branches-2.png)

### Figure 30 - Server (Remote) and local repositories after cloning

![Server and local repositories after cloning](https://github.com/aridiosilva/git/blob/main/remote-branches-1.png)

### Figure - Git fetch updates your remote-tracking branches

![Figure 32. git fetch updates your remote-tracking branches](https://github.com/aridiosilva/git/blob/main/remote-branches-3.png)

## GitHub Markup Language

- [Github Markup Language](https://guides.github.com/features/mastering-markdown/#:~:text=Markdown%20is%20a%20lightweight%20and,writing%20on%20the%20GitHub%20platform.)

## Git Glossary

(https://git-scm.com/docs/gitglossary)

## Git Reference

(https://git-scm.com/docs)
(https://training.github.com/downloads/github-git-cheat-sheet/)

## List of All Commands of Git

(https://git-scm.com/docs/git#_git_commands)

## Book Pro Git
Book 2nd Edition (2014) - The entire Pro Git book, written by Scott Chacon and Ben Straub and published by Apress, is available here. All content is licensed under the Creative Commons Attribution Non Commercial Share Alike 3.0 license. Print versions of the book are available on Amazon.com.

- [download eBook](https://github.com/progit/progit2-pt-br/releases/download/2.1.28/progit_v2.1.28.pdf)
- [Read the Book Pro Git Edition 2 ONLINE](https://git-scm.com/book/pt-br/v2)
- [Basics of Getting a Git Repository](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository)

## EGIT User Guide for ECLIPSE IDE 2020-12

- [USer Guide of Git for usewith ECLIPSE IDE](https://github.com/aridiosilva/gamificacao/blob/master/Gamificacao/help/EGit%20User%20Guide%20-%20Git%20for%20ECLIPSE%20IDE%202020-12%20in%2020-DEC-2020.pdf)

## Configure tooling

Configure user information for all local repositories

- **$ git config --global user.name "[name]"** - Sets the name you want attached to your commit transactions
- **$ git config --global user.email "[email address]"** - Sets the email you want attached to your commit transactions
- **$ git config --global color.ui auto** - Enables helpful colorization of command line output

## Create repositories

A new repository can either be created locally, or an existing repository can be cloned. When a repository was initialized locally, you have to push it to GitHub afterwards.

- **$ git init** - The git init command turns an existing directory into a new Git repository inside the folder you are running this command. After using the git init command, link the local repository to an empty GitHub repository using the following command:
- **$ git remote add origin [url]** - Specifies the remote repository for your local repository. The url points to a repository on GitHub.
- **$ git clone [url]** - Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits

## The .gitignore file

Sometimes it may be a good idea to exclude files from being tracked with Git. This is typically done in a special file named .gitignore. You can find helpful templates for .gitignore files at github.com/github/gitignore.

## Make changes

Browse and inspect the evolution of project files

- **$ git log** - Lists version history for the current branch
- **$ git log --follow [file]** - Lists version history for a file, beyond renames (works only for a single file)
- **$ git diff [first-branch]...[second-branch]**  - Shows content differences between two branches
- **$ git show [commit]** - Outputs metadata and content changes of the specified commit
- **$ git add [file]** -  Snapshots the file in preparation for versioning
- **$ git commit -m "[descriptive message]"** - Records file snapshots permanently in version history

## Synchronize changes

Synchronize your local repository with the remote repository on GitHub.com:

- **$ git fetch**    -  Downloads all history from the remote tracking branches
- **$ git merge**    -  Combines remote tracking branches into current local branch
- **$ git push**     -  Uploads all local branch commits to GitHub
- **$ git pull**     -  Updates your current local working branch with all new commits from the corresponding remote branch on GitHub. git pull is a combination of git fetch and git merge

## Redo commits

Erase mistakes and craft replacement history

- **$ git reset [commit]** - Undoes all commits after [commit], preserving changes locally
- **$ git reset --hard [commit]** - Discards all history and changes back to the specified commit
- **CAUTION!** Changing history can have nasty side effects. If you need to change commits that exist on GitHub (the remote), proceed with caution. If you need help, reach out at github.community or contact support.

## Key Concepts in GitHub and Git

There are a number of key concepts that you’ll need to understand to work effectively with Git and GitHub. Here is a list of some of the most common terms with a short
description of each and an example of how they might be used in conversation:

### Commit

A Git object, a snapshot of your entire repository compressed into a SHA.

Whenever you save your changes to one or more files to history in Git, you create a new commit. Example usage: “Let’s commit these changes and push them up to
GitHub.”

### Commit message

Every time you make a commit, you need to supply a message that describes why the change was made. That commit message is invaluable when trying to understand
later why a certain change was implemented. Example usage: “Make sure to include Susan’s comment about the new SEC guidelines in the commit message.”

### Branch

A Git object, a snapshot of your entire repository compressed into a SHA.  An independent series of commits off to one side that you can use to try out an experiment or create a new feature. Example usage: “Let’s create a branch to implement the new search functionality.”

Branches are an important part of working with Git. Any commits you make will be made on the branch you’re currently “checked out” to. Use git status to see which branch that is.

- **$ git branch [branch-name]**     - Creates a new branch
- **$ git checkout [branch-name]**   - Switches to the specified branch and updates the working directory
- **$ git merge [branch]**           - Combines the specified branch’s history into the current branch. This is usually done in pull requests, but is an important Git operation.
- **$ git branch -d [branch-name]**  - Deletes the specified branch

### Clone

A local version of a repository, including all commits and branches.

### Fork

A copy of a repository on GitHub owned by a different user

### Head

Representing your current working directory, the HEAD pointer can be moved to different branches, tags, or commits when using git checkout

### Master branch (master)

Whenever you create a new Git project, there is a default branch created that is called master. This is the branch that your work should end up on eventually once it’s ready
to push to production. Example usage: “Remember never to commit directly to master.”

### Feature (or topic) branch

Whenever you’re building a new piece of functionality, you’ll create a branch to work on it. That’s called a feature branch. Example usage: “We’ve got way too many feature
branches. Let’s focus on getting one or two of these finished and into production.”

### Release branch

If you have a manual QA process or have to support old versions of your software for your customers, you might need a release branch as a place to make any necessary fixes or updates. There is no technical difference between a feature or release branch, but the distinction is useful when talking about a project with your team. Example usage: “We’ve got to fix the security bug on all of our supported release branches.”

### Remote

A common repository on GitHub that all team members use to exchange their changes.

### Merge

This is a way to take completed work from one branch and incorporate it into another branch. Most commonly you’ll merge a feature branch into the master
branch. Example usage: “Great job on the ‘my account’ feature. Could you merge it into master so we can push it to production?”

### Tag

A reference to a specific historic commit. Most often used to document production releases so you know exactly which versions of the code went into production and
when. Example usage: “Let’s tag this release and push it to production.” 

### Check out

To go to a different version of the project’s history to see the files as of that point in time. Most commonly you’ll check out a branch to see all of the work that has been
done on it, but any commit can be checked out. Example usage: “Could you check out the last release tag? There’s a bug in production that I need you to replicate and fix.”

### Pull request

A place to compare and discuss the differences introduced on a branch with reviews, comments, integrated tests, and more.

Originally, a pull request was used to request that someone else review the work you completed on a branch and then merge it into master. Now, pull requests are often
used earlier in the process to start a discussion about a possible feature. Example usage: “Go create a pull request for the new voting feature so we can see what the rest of
the team thinks about it.” Pull requests give you a sense of the current work in progress.

Labels of differents types of pull requested allowed in GituHUb are:

   - **bug** - Something isn't working
   - **duplicate** -This issue or pull request already exists
   - **enhancement** - New feature or request
   - **good first issue** - Good for newcomers
   - **help wanted** - Extra attention is needed
   - **invalid** - This doesn't seem right
   - **question** - Further information is requested
   - **wontfix** - This will not be worked on

Pull requests help you collaborate on code with other people. As pull requests are created, they’ll appear here in a searchable and filterable list. To get started, you should create a pull request.

### Issue

GitHub has a feature called Issues that can be used to discuss features, track bugs, or both. Example usage: “You’re right, the login doesn’t work on an iPhone. Could you create
an issue on GitHub documenting the steps to replicate the bug?”. 

Issues are used to track todos, bugs, feature requests, and more. As issues are created, they’ll appear here in a searchable and filterable list. To get started, you should create an issue.

### Wiki

Originally developed by Ward Cunningham, wikis are a lightweight way of creating web pages with simple links between them. GitHub projects often use wikis for documentation. Example usage: “Could you add a page to the wiki to explain how to configure the project to run on multiple servers?”

### Clone

Often you’ll want to download a copy of a project from GitHub so you can work on it locally. The process of copying the repository to your computer is called cloning. Example usage: “Could you clone the repo, fix the bug, and then push the fix back up to GitHub later tonight?”

### Fork

Sometimes you don’t have the necessary permission to make changes directly to a project. Perhaps it’s an open source project written by people you don’t know or it’s a project written by another group at your company that you don’t work with much. If you want to submit changes to such a project, first you need to make a copy of the project under your user account on GitHub. That process is called forking the repository. You can then clone it, make changes, and submit them back to the original project using a pull request. Example usage: “I’d love to see how you’d rewrite the home page marketing copy. Fork the repo and submit a pull request with your proposed
changes.”

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

## Git Commands by Group

### Setup and Config

- git
- config
- help
- bugreport

### Getting and Creating Projects

- init
- clone

### Basic Snapshotting

- add
- status
- diff
- commit
- notes
- restore
- reset
- rm
- mv

### Branching and Merging

- branch
- checkout
- switch
- merge
- mergetool
- log
- stash
- tag
- worktree

### Sharing and Updating Projects

- fetch
- pull
- push
- remote
- submodule

### Inspection and Comparison

- show
- log
- diff
- difftool
- range-diff
- shortlog
- describe

### Patching

- apply
- cherry-pick
- diff
- rebase
- revert

### Debugging

- bisect
- blame
- grep

### Guides

- gitattributes
- Command-line interface conventions
- Everyday Git
- Frequently Asked Questions (FAQ)
- Glossary
- Hooks
- gitignore
- gitmodules
- Revisions
- Submodules
- Tutorial
- Workflows
- All guides...

### Email

- am
- apply
- format-patch
- send-email
- request-pull

### External Systems

- svn
- fast-import

### Administration

- clean
- gc
- fsck
- reflog
- filter-branch
- instaweb
- archive
- bundle

### Server Admin

- daemon
- update-server-info

### Plumbing Commands

- cat-file
- check-ignore
- checkout-index
- commit-tree
- count-objects
- diff-index
- for-each-ref
- hash-object
- ls-files
- ls-tree
- merge-base
- read-tree
- rev-list
- rev-parse
- show-ref
- symbolic-ref
- update-index
- update-ref
- verify-pack
- write-tree

