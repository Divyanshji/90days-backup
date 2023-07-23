---
title: "Deep Dive in Git & GitHub for DevOps Engineers."
datePublished: Sun Jul 23 2023 16:31:18 GMT+0000 (Coordinated Universal Time)
cuid: clkfnowsj00000aig49t84mdr
slug: deep-dive-in-git-github-for-devops-engineers
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1689965164927/5f0418d6-1e6b-412f-8d6d-fad8228187eb.png
tags: github, devops, 90daysofdevops, day9, divyanshjain

---

## Introduction

Welcome to Day 8 of the #90DaysOfDevOps challenge! Today, we'll learn about GIT and GitHub. We often use these words interchangeably, but they both are not the same. In the fast-paced world of software development, collaboration, version control, and continuous integration are vital components of successful DevOps practices. Git and GitHub have emerged as essential tools in the DevOps engineer's weapons, enabling teams to streamline workflows, improve code quality, and foster efficient collaboration. In this blog, we'll explore the fundamentals of Git and GitHub, their significance in the DevOps ecosystem, and how they revolutionize the way development teams work together to deliver exceptional software.

## What is GIT and Why it is important?

**Git :** Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency. git also used for source code management.

Git is used to tracking changes in the source code, enabling multiple developers to work together on non-linear development. With Git, you can keep a record of who made changes to what part of a file, and you can revert back to earlier versions of the file if needed. Git also makes it easy to collaborate with others, as you can share changes and merge the changes made by different people into a single version of a file.

### **What is difference Between Main Branch and Master Branch?**

There is no difference between main and master branch in git. Main or Master branch is a default branch when you create a repository. GitHub now use **main** as a it's **default branch**. while others still use master branch as a default branch.

## Can you explain the difference between Git and GitHub?

**Git:**

Git is a distributed version control system, tracking changes in any set of files, usually used for coordinating work among programmers collaboratively developing source code during software development. Git is installed and maintained on your local system. Git is a command-line tool.

**GitHub:**

GitHub is a cloud-based platform that provides hosting for version control using Git. It is a service we use to store our project files. GitHub is designed as a git repository hosting service. GitHub is a graphical user interface.

## How do you create a new repository on GitHub?

step 1: Sign in to your GitHub account using your username and password.

step 2: Once you are signed in, click on the "+" icon in the top-right corner of the GitHub homepage. From the dropdown menu, select "New repository." or, go to repositories and click on 'new' in the top right corner.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689961746389/d2befa9d-1c71-4e0b-83c6-020a082433c1.png align="center")

Step 3: **Set up the repository**: Now Add the repository name and other details like whether you want to keep it public(publically accessible) or private repo.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689961836840/912c2096-037b-41ad-bc4c-44975c4e72ad.png align="center")

Then click on 'create repository'

you have successfully created a repository.

### What is difference between local & remote repository? How to connect local to remote?

Git local repository is the one on which we will make local changes, typically this local repository is on our computer.

Git remote repositories are hosted on a server that is accessible for all team members. 

A git **remote command** is used to make the remote connections such as connecting a Git local repository with GitHub remote repository.

1.**git remote add origin** [**https://github.com/YOUR-USERNAME/YOUR-REPOSITORY**](https://github.com/YOUR-USERNAME/YOUR-REPOSITORY)

2.**git push origin master**