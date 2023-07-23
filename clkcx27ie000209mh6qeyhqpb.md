---
title: "Basic Git & GitHub for DevOps Engineers."
datePublished: Fri Jul 21 2023 18:30:17 GMT+0000 (Coordinated Universal Time)
cuid: clkcx27ie000209mh6qeyhqpb
slug: basic-git-github-for-devops-engineers
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1689957737278/ba5f1f26-5092-4914-b1a1-288ce2495d2d.png
tags: github, devops, 90daysofdevops, day8, divyanshjain

---

## 🌟Introduction🌟

Welcome to Day 8 of the #90DaysOfDevOps challenge! Today, we'll learn about GIT and GitHub. We often use these words interchangeably, but they both are not the same. In the fast-paced world of software development, collaboration, version control, and continuous integration are vital components of successful DevOps practices. Git and GitHub have emerged as essential tools in the DevOps engineer's weapons, enabling teams to streamline workflows, improve code quality, and foster efficient collaboration. In this blog, we'll explore the fundamentals of Git and GitHub, their significance in the DevOps ecosystem, and how they revolutionize the way development teams work together to deliver exceptional software.

## 🌟Git and GitHub🌟

## 🔑What is Git?

Git is a distributed version control system that allows multiple developers to work together on the same project without stepping on each other's toes. It gives you the superpower to manage and track changes to your code, making it easier to fix bugs, experiment with new features, and seamlessly roll back to previous versions if needed. 😎 No more living in fear of breaking the code! Git has your back! 💪

### 🔑What is GitHub?

GitHub is a web-based platform that provides hosting for version control using Git. It is a subsidiary of Microsoft, and it offers all of the distributed version control and source code management (SCM) functionality of Git as well as adding its own features. GitHub is a very popular platform for developers to share and collaborate on projects, and it is also used for hosting open-source projects.

## 🌟What is Version Control?

Version control is a system that tracks changes to a file or set of files over time so that you can recall specific versions later. It allows you to revert files back to a previous state, revert the entire project back to a previous state, compare changes over time, see who last modified something that might be causing a problem, who introduced an issue and when, and more.

There are two main types of version control systems: centralized version control systems and distributed version control systems.

1. A **centralized version control system (CVCS)** uses a central server to store all the versions of a project's files. Developers "check out" files from the central server, make changes, and then "check in" the updated files. Examples of CVCS include Subversion and Perforce.
    
2. A **distributed version control system (DVCS)** allows developers to "clone" an entire repository, including the entire version history of the project. This means that they have a complete local copy of the repository, including all branches and past versions. Developers can work independently and then later merge their changes back into the main repository. Examples of DVCS include Git, Mercurial, and Darcs.
    

### 🔑Why we use distributed version control over centralized version control?

1. **Better collaboration:** In a DVCS, every developer has a full copy of the repository, including the entire history of all changes. This makes it easier for developers to work together, as they don't have to constantly communicate with a central server to commit their changes or to see the changes made by others.
    
2. **Improved speed:** Because developers have a local copy of the repository, they can commit their changes and perform other version control actions faster, as they don't have to communicate with a central server.
    
3. **Greater flexibility:** With a DVCS, developers can work offline and commit their changes later when they do have an internet connection. They can also choose to share their changes with only a subset of the team, rather than pushing all of their changes to a central server.
    
4. **Enhanced security:** In a DVCS, the repository history is stored on multiple servers and computers, which makes it more resistant to data loss. If the central server in a CVCS goes down or the repository becomes corrupted, it can be difficult to recover the lost data.
    

Overall, the decentralized nature of a DVCS allows for greater collaboration, flexibility, and security, making it a popular choice for many teams.

![Version Control | Centralized vs Distributed System - YouTube](https://i.ytimg.com/vi/MAoAY1wYJuE/maxresdefault.jpg align="left")

## 🌟Install Git on your computer

<mark>You can download it from the official website at</mark>

[**https://git-scm.com/downloads**](https://git-scm.com/downloads)

```plaintext
sudo apt-get update && sudo apt-get install git 
git --version
```

## 🌟**Create a free account on GitHub**

`You can signup from:` [**https://github.com/**](https://github.com/)

### 🔑**You need to know some basic commands of git**

<table><tbody><tr><td colspan="1" rowspan="1"><p><strong>Command</strong></p></td><td colspan="1" rowspan="1"><p><strong>Description</strong></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git init</code></p></td><td colspan="1" rowspan="1"><p>Initializes a new Git repository in the current directory.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git clone</code></p></td><td colspan="1" rowspan="1"><p>Creates a local copy of a remote repository.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git add</code></p></td><td colspan="1" rowspan="1"><p>Adds changes or new files to the staging area for the next commit.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git commit</code></p></td><td colspan="1" rowspan="1"><p>Records changes to the repository with a commit message.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git status</code></p></td><td colspan="1" rowspan="1"><p>Shows the status of the working directory and staging area.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git push</code></p></td><td colspan="1" rowspan="1"><p>uploads local commits to a remote repository.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git pull</code></p></td><td colspan="1" rowspan="1"><p>Fetches and merges changes from a remote repository.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git branch</code></p></td><td colspan="1" rowspan="1"><p>Lists, creates, or deletes branches in the repository.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git checkout</code></p></td><td colspan="1" rowspan="1"><p>Switches to a different branch or restores files from a commit.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git merge</code></p></td><td colspan="1" rowspan="1"><p>Combines changes from one branch into another branch.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git log</code></p></td><td colspan="1" rowspan="1"><p>Displays a history of commits in the repository.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git remote</code></p></td><td colspan="1" rowspan="1"><p>Manages remote repositories linked to the local repository.</p></td></tr></tbody></table>

## 🌟Create a new repository on GitHub and clone it to your local machine

step 1: Sign in to your GitHub account using your username and password.

step 2: Once you are signed in, click on the "+" icon in the top-right corner of the GitHub homepage. From the dropdown menu, select "New repository." or, go to repositories and click on 'new' in the top right corner.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689961746389/d2befa9d-1c71-4e0b-83c6-020a082433c1.png align="center")

Step 3: **Set up the repository**: Now Add the repository name and other details like whether you want to keep it public(publically accessible) or private repo.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689961836840/912c2096-037b-41ad-bc4c-44975c4e72ad.png align="center")

Then click on 'create repository'

you have successfully created a repository.

step 4: After creating the Repository it will look something like this :

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689962026138/d3a4379b-16d0-4bd6-8d24-fe40f4e9f5e9.png align="center")

### 🔑Clone Repo to local machine

**step1**: click on **<mark>&lt;&gt;code</mark>**, after that, we can see a path, and copy that path

**step 2**: lets go into your local machine .

**step 3**: git clone &lt;paste\_the\_copied\_link\_here&gt;

it will clone your repository into your local.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689962175583/963f792a-b8b2-4aa8-8980-8efa44fe7230.png align="center")

### 🔑Make some changes to a file in the repository and commit them to the repository using Git

Create a few files or do the code you want to and then commit them.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689962375289/645c8240-61c3-479e-afa1-64e9ad3abf46.png align="center")

We have create 2 files and added few line of code in each file.

We will now commit these changes but in order to commit we will add them to staging directory and then commit them.

![What's the difference between HEAD, working tree and index, in Git? - Stack  Overflow](https://i.stack.imgur.com/CYO5D.jpg align="left")

You can see in picture about is **Git Working Tree.**

In the below screenshot using `git status` command you can track your code stage, and track them using `git add` command. This is following command useful for committing code.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689963349130/79b2f31d-7374-42be-8876-07a384635db5.png align="center")

Remember we only committed in local repo not the remote repo(GitHub).

### 🔑Push the changes back to the repository on GitHub

We need to push this code in order to commit code to remote repo.

```plaintext
git push origin <branch-name>
```

## 🌟Conclusion

Congratulations, dear reader! 🎊 You've mastered the art of Git and GitHub, joining the ranks of legendary DevOps engineers! 🎓 Embrace version control and collaboration, and your coding adventures shall know no bounds!

May your repositories be evergreen, and your codebase shine brightly among the stars! 🌟 Happy coding! 🚀🔥

Remember, the magical world of DevOps holds infinite wonders, so stay curious and keep learning! 🌈💻