---
title: "Advance Git & GitHub for DevOps Engineers: Part-2"
datePublished: Tue Jul 25 2023 17:13:21 GMT+0000 (Coordinated Universal Time)
cuid: clkik2orj000m09l74jiy0dcr
slug: advance-git-github-for-devops-engineers-part-2
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1690305159632/0bcd0830-4406-458b-a846-5b264f970c32.jpeg
tags: git, devops, 90daysofdevops, advancegit, divyanshjain

---

## 🌟Introduction🌟

Welcome to Day 11 of the #90DaysOfDevOps challenge! Today, we'll learn about GIT Advance concepts. In the fast-paced world of software development, collaboration, version control, and continuous integration are vital components of successful DevOps practices.

## What is Git Stash?

1. Git stash is a command that allows you to temporarily save changes you have made in your working directory, without committing them.
    
2. This is useful when you need to switch to a different branch to work on something else, but you don't want to commit the changes you've made in your current branch yet.
    
3. To use Git stash, you first create a new branch and make some changes to it.
    
4. Then you can use the command git stash to save those changes.
    
5. This will remove the changes from your working directory and record them in a new stash.
    
6. You can apply these changes later.
    
7. git stash list command shows the list of stashed changes.
    
8. You can also use git stash drop to delete a stash and git stash clear to delete all the stashes.
    
9. Stashed changes are saved separately from your commits.
    
10. You can use `git stash save` to create a new stash with an optional message.
    
11. Stashes can be listed using `git stash list` and applied with `git stash apply`.
    
12. Stashes are helpful when you need to switch branches or perform other operations without committing your changes.
    

![Solution:Cannot pull with rebase: You have unstaged changes in Github |  CreativeDev](https://www.thecreativedev.com/wp-content/uploads/2015/04/git-cannot-pull-with-rebase-you-have-unstaged-changes-545x300.png align="left")

**Some git stash commands**

<table><tbody><tr><td colspan="1" rowspan="1"><p><strong>Command</strong></p></td><td colspan="1" rowspan="1"><p><strong>Description</strong></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git stash save "message"</code></p></td><td colspan="1" rowspan="1"><p>Save changes to a new stash with an optional message.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git stash list</code></p></td><td colspan="1" rowspan="1"><p>List all stashes with their references.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git stash show stash@{n}</code></p></td><td colspan="1" rowspan="1"><p>Show changes stored in a specific stash.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git stash apply stash@{n}</code></p></td><td colspan="1" rowspan="1"><p>Apply changes from a specific stash to the working directory.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git stash pop stash@{n}</code></p></td><td colspan="1" rowspan="1"><p>Apply changes from a stash and remove it from the stash list.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git stash branch branchname stash@{n}</code></p></td><td colspan="1" rowspan="1"><p>Create a new branch from a stash and apply it.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git stash drop stash@{n}</code></p></td><td colspan="1" rowspan="1"><p>Delete a specific stash.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git stash clear</code></p></td><td colspan="1" rowspan="1"><p>Delete all stashes.</p></td></tr></tbody></table>

## What is Cherry-pick?

1. Git cherry-pick is a command that allows you to select specific commits from one branch and apply them to another.
    
2. This can be useful when you want to selectively apply changes that were made in one branch to another.
    
3. To use git cherry-pick, you first create two new branches and make some commits to them.
    
4. You can cherry-pick a single commit or multiple commits in a specified order.
    
5. Then you use `git cherry-pick <commit_hash>` command to select the specific commits from one branch and apply them to the other.
    

![How To Cherry Pick Git Commits | When & How to use a Git Cherry Pick  Commit? – Junos Notes](https://www.junosnotes.com/wp-content/uploads/2021/07/how-do-i-cherry-pick-a-commit-in-Git.png align="left")

**Some git cherrypick commands in git**

<table><tbody><tr><td colspan="1" rowspan="1"><p><strong>Command</strong></p></td><td colspan="1" rowspan="1"><p><strong>Description</strong></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git cherry-pick &lt;commit&gt;</code></p></td><td colspan="1" rowspan="1"><p>Applies the changes of the specified commit onto the current branch.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git cherry-pick &lt;start&gt;..&lt;end&gt;</code></p></td><td colspan="1" rowspan="1"><p>Applies the changes of a range of commits onto the current branch. The range includes both the start and end commits.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git cherry-pick -n &lt;commit&gt;</code></p></td><td colspan="1" rowspan="1"><p>Applies the changes of the specified commit onto the current branch but does not create a new commit. Allows making further modifications before committing.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git cherry-pick --continue</code></p></td><td colspan="1" rowspan="1"><p>Completes the cherry-pick operation after resolving conflicts.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git cherry-pick --abort</code></p></td><td colspan="1" rowspan="1"><p>Aborts the cherry-pick operation and restores the branch to its original state before the cherry-pick started.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git cherry-pick --quit</code></p></td><td colspan="1" rowspan="1"><p>Aborts the cherry-pick operation but keeps any changes that have been applied. Useful when you want to save the changes but not continue with the cherry-pick.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git cherry-pick --edit &lt;commit&gt;</code></p></td><td colspan="1" rowspan="1"><p>Opens the commit message in an editor, allowing you to modify it before committing the cherry-picked changes.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git cherry-pick --signoff &lt;commit&gt;</code></p></td><td colspan="1" rowspan="1"><p>Appends a "Signed-off-by" line with your name and email to the commit message of the cherry-picked changes.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git cherry-pick --strategy=recursive &lt;commit&gt;</code></p></td><td colspan="1" rowspan="1"><p>Specifies a merge strategy to be used during the cherry-pick operation. The default is the 'recursive' strategy.</p></td></tr><tr><td colspan="1" rowspan="1"><p><code>git cherry-pick --no-commit &lt;commit&gt;</code></p></td><td colspan="1" rowspan="1"><p>Applies the changes of the specified commit but does not automatically create a new commit. Allows making further modifications or combining changes.</p></td></tr></tbody></table>

## **What is Resolving Conflicts?**

1. In Git, conflicts can arise when two or more developers make changes to the same file(s) and attempt to merge their changes together. Git is designed to detect and highlight such conflicts, and it is up to the developers to resolve them manually.
    
2. Resolving conflicts in Git involves identifying the conflicting changes and deciding how to integrate them into a new, merged version of the file. This can be done using Git's built-in merge tools or manually by editing the conflicting sections of the file.
    
    ![How to Resolve Merge Conflicts in Git – A Practical Guide with Examples](https://www.freecodecamp.org/news/content/images/2022/05/image-45.png align="left")
    

### **✔️Task 1:**

1. Create a new branch and make some changes to it.
    
    ```plaintext
      git checkout -b feature
      git branch
      vim version01.txt
      git add .
    ```
    
2. Use git stash to save the changes without committing them.
    
    ```plaintext
      git stash
      git status
    ```
    
3. Switch to a different branch, make some changes and commit them.
    
    ```plaintext
      git checkout development
      vim version01.txt
      git add .
      git commit -m "version file commited"
    ```
    
4. Use git stash pop to bring the changes back and apply them on top of the new commits.
    

```plaintext
 git stash list
 git stash pop
 git add .
 git commit -m "git stash file commited"
 git log --oneline
```

### **✔️Task 2:**

1. In version01.txt of the development branch add the below lines after "This is the bug fix in development branch" that you added in Day10 and reverted to this commit.
    
    ```plaintext
       git checkout dev
       vim version01.txt  :- "This is the bug fix in development branch"
       cat version01.txt 
       git add version01.txt 
       git commit -m "commited file on dev"
    ```
    
2. Line2&gt;&gt; After bug fixing, this is the new feature with minor alteration
    
    Commit this with the message "Added feature2.1 in development branch"
    
    ```plaintext
      vim version01.txt :- "After bug fixing, this is the new feature with minor alteration"
      git add version01.txt 
      git commit -m "Added feature 2.1 in development branch"
    ```
    
3. Line3&gt;&gt; This is the advancement of previous feature
    
    Commit this with the message "Added feature2.2 in development branch"
    
    ```plaintext
      vim version01.txt  :- "This is the advancement of  previous feature "
      git add version01.txt 
      git commit -m "Added feature 2.2 in development branch"
    ```
    
4. Line4&gt;&gt; Feature 2 is completed and ready for release
    
    Commit this with the message "Feature2 completed"
    
    ```plaintext
      vim version01.txt  :- "Feature 2 is completed and ready for release"
      git add version01.txt 
      git commit -m "Feature2 completed"
    ```
    
5. All these commits messages should be reflected in the Production branch too which will come out from the Master branch.
    
    ```plaintext
      git checkout prod
      git rebase dev
      git log --oneline
    ```
    

### **✔️Task 3:**

1. In Production branch Cherry pick Commit “Added feature2.2 in development branch” and added below lines in it:
    
    ```plaintext
      git log --oneline
      git cherry-pick <commit_id>
      vi version01.txt
    ```
    
2. Line to be added after Line3&gt;&gt; This is the advancement of previous feature
    
    ```plaintext
      vi version01.txt :- "This is the advancement of previous feature"
      git add version01.txt
      git commit -m "adv feature"
    ```
    

Line4&gt;&gt;Added few more changes to make it more optimized. Commit: Optimized the feature

```plaintext
  vi version01.txt  :- "Added few more changes to make it more optimized"
  git add version01.txt
  git commit -m "Optimized the feature"
```

## Conclusion

Congratulations, dear reader! 🎊 You've mastered the art of Git and GitHub, joining the ranks of legendary DevOps engineers! 🎓 Embrace version control and collaboration, and your coding adventures shall know no bounds!

Stay in the loop with my latest insights and articles on cloud ☁️ and DevOps 🚀 by following me on Hashnode, LinkedIn ([**www.linkedin.com/in/Divyansh-Jain**](http://www.linkedin.com/in/divyansh-jain-03496617a/)), and GitHub ([**https://github.com/Divyansh-jain**](https://github.com/Divyanshji)).

**Thank you for reading!** 🙏 Your support means the world to me. Let's keep learning, growing, and making a positive impact in the tech world together.