# Week 8 -  Intro to Version Control

**Version control** (also known as **source control management**) is a system that records changes to a file or set of files over time so that you can recall specific versions later. Many popular systems include aspects of version control built-in to the software like word processors (ie. Google Docs, etc) and content management systems (ie. WordPress, etc).

- [Wikipedia: Revision Control](https://en.wikipedia.org/wiki/Revision_control)
- [Git SCM: Getting started - about version control](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)


There's multiple types of version control systems available, including [CVS](http://www.nongnu.org/cvs/), [SVN](http://subversion.apache.org/), [Git](https://git-scm.com/) et al. Each system is catered to a specific type of workflow for collaboration, but generally all provide the same file versioning/history capabilities.

- [Wikipedia: List of types of version control](https://en.wikipedia.org/wiki/List_of_revision_control_software)

**Video: [Git Basics: What is Version Control?](https://vimeo.com/41027679)**
[![What is Version Control](images/git/what-is-version-control.png)](https://vimeo.com/41027679)

#### What is Git/GitHub?
[![Git SCM Logo](images/git/git-logo.png)](https://git-scm.com/)

**[Git](https://git-scm.com/) is the fastest growing and most popular version control system used to track and share documents today.**

Git provides common version control capabilities, but with it's own, unique organizational workflow. Git's [branching model concept](#branch) encourages a *feature-based workflow*, allowing people to seamlessly switch back and forth between different features they're working on and experiment without impacting the integrity of their code-base.

Git also allows groups of people to work on the same documents (often code) at the same time, and without stepping on each other's toes. It's a distributed, version control system.

[![Github](images/git/github-logo.png)](https://github.com/)

**[GitHub](https://github.com/) is a web-based, Git repository hosting service. _(ie. a 'hub' for Git repo's, get it?)_**

Unlike Git, which is strictly a command-line (CLI) tool, GitHub provides a web-based graphical interface and desktop client for managing Git repositories.

GitHub also provides access control and several collaboration features such as bug tracking, feature requests, task management, and wikis for every project.

##### Download [GitHub Desktop app](https://desktop.github.com/)
  - [GitHub for Mac](https://central.github.com/mac/latest)
  - [GitHub for PC](https://github-windows.s3.amazonaws.com/GitHubSetup.exe)

*The GitHub Desktop app should already be installed on the KOPIKO 202 & KOA 103 studio classroom computers.*

#### Git/GitHub Concepts
- [Git: The advantages of Git compared to other source control systems](https://git-scm.com/about/)
- [Git: Getting started - Git basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)
- [GitHub Help](https://help.github.com/)

##### Repository
A Git repository is nothing more than a directory (ie. folder) on a computer. Any file in your 'repo' will be tracked and a history of the changes will be recorded (unless [explicitly ignored](http://git-scm.com/docs/gitignore), which we'll talk about a bit later).

##### Branch
A Git branch is a working copy of your code, *in a specific state*. When you're working on a project, you're going to have a bunch of different features or ideas in progress at any given time – some of which are ready to go, and others which are not. Branching exists to help you manage this workflow.

##### Commit
A commit saves your current changes to your current branch. Once you start making changes in a repository, Git will start tracking those changes. Whenever you add, edit, or delete a file, you're making a commit, and adding them to your branch. This process of adding commits keeps track of your progress as you work on a feature branch.

##### Push/Pull (Sync)
A good practice in web development is to create backups of your projects. This is where _**GitHub**_ comes in, as a central repository hosting service for Git projects. Once you've wrapped up with your coding session, it's a good idea to sync your local repository with GitHub so all of your code changes are archived. If you're working on a team or between multiple machines, it's also a good idea to sync your local repository before you start working as well.

##### Pull Request
In the *[GitHub development workflow](#github-development-workflow)*, theres a `master` branch that keeps the final record of the code ready for deployment. To get code from our feature branches in to our master branch, we need to make a pull request.

##### Merge
In Git, merging brings the changes in two branches together. A pull request is a request to merge a set of commits from one branch in to another. Merges can be performed on your local machine to combine changes from two feature branches before syncing, and making a pull request to the `master` branch on Github.

#### GitHub development workflow

As we go through the semester, we'll cover different aspects of Git & GitHub within our workflow. At a [high-level](https://en.wikipedia.org/wiki/High-_and_low-level), we'll be following the [GitHub-Flow](https://guides.github.com/introduction/flow/) methodology for development with some slight adjustments for this course.

- Anything in the `master` branch is deployable
- To work on something new, create a descriptively named branch off of `master` (ie: `home-page-bug-fix`)
- Commit to that branch locally and regularly push (ie. sync) your work to the same named branch on GitHub
- When you need feedback or help, create an issue and mention myself and/or another student using the @username syntax (ie, @epilande)
- When you are ready to submit your code assignment, create a pull request


### Reference
- [Why Use a Version Control System?](https://www.git-tower.com/learn/git/ebook/command-line/basics/why-use-version-control)
- [Try Git (Command-line)](https://try.github.io/levels/1/challenges/1)

