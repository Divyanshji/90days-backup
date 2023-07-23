---
title: "Day 3 Task: Basic Linux Commands (Part 2)"
datePublished: Mon Jul 17 2023 14:07:18 GMT+0000 (Coordinated Universal Time)
cuid: clk6xwlxp000009mpa9b5coqh
slug: day-3-task-basic-linux-commands-part-2
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1689595925725/8e096bbb-2556-4445-a2ea-17bedb043d7e.png
tags: linux, devops, 90daysofdevops, day3

---

## Introduction

Welcome to Day 3 of the #90DaysOfDevOps challenge! Today, we'll explore more Linux commands, like magical keys unlocking every DevOps engineer's potential! Mastering Linux commands is a skill that opens up a world of possibilities.🚀🗺️💻 Whether you're a developer, system administrator, or simply someone who wants to harness the power of the terminal, understanding these commands will empower you to work efficiently, automate tasks, and take control of your Linux experience.

So, grab your virtual terminal, put on your command-line wizard hat, and let's embark on this exciting adventure together.

1. ## To view what's written in a file.
    
    To view the contents of a file in Linux, you can use the "**cat**" command. For example, let's say you have a file named "first.txt" To view what's written in this file, open your terminal and write **cat first.txt**:
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689596812416/d54d6c19-cc6a-4dbe-a356-edeec8e1928a.png align="center")
    
2. ## To change the access permissions of files.
    
    To change the access permissions of files interactively, you can use the `chmod` command in Linux. 🚀🔐
    
    The `chmod` command allows you to modify the read, write, and execute permissions of files and directories. To use it interactively, follow these steps:
    
    1. Open the terminal and navigate to the directory where the file is located. 📁💻
        
    2. Type the following command, replacing `filename` with the actual name of the file you want to modify:
        
        ```plaintext
        chmod +rwx filename
        ```
        
        This command gives the file read, write, and execute permissions to the owner, group, and others.
        
    3. Now, the file's permission has changed, and you can customize it further based on your needs. Let's break down the command:
        
        * `+rwx`: Adds read, write, and execute permissions.
            
        * `-rwx`: Removes read, write, and execute permissions.
            
        * `r`: Represents read permission.
            
        * `w`: Represents write permission.
            
        * `x`: Represents execute permission.
            
    4. After executing the initial `chmod` command, you can modify the permissions interactively by typing:
        
        ```plaintext
        bashCopy codechmod ugo+/-permissions filename
        ```
        
        * `u`: Represents the file owner.
            
        * `g`: Represents the file group.
            
        * `o`: Represents others (users not in the owner or group).
            
        * `+/-permissions`: Adds or removes specific permissions.
            
    
    For example, to remove execute permission from others (users not in the owner or group), you would type:
    
    ```plaintext
    bashCopy codechmod o-x filename
    ```
    
    Remember, these commands modify permissions on a file. Exercise caution while changing permissions, as incorrect settings can affect the functionality and security of your files.
    
    Now you're equipped with the knowledge to interactively change access permissions using the `chmod` command. Enjoy the flexibility and control it brings to your Linux experience! 🔒🖥️
    
3. ## To check which commands you have run till now.
    
    To check the commands you have run in the current terminal session in Linux, you can use the "history" command. 📜
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689597449895/4c327579-4eda-4b5f-a5bc-be9721f3e4f5.png align="center")
    
4. ## To remove a directory/ Folder.
    
    Removing a directory or folder in Linux is done using the "**rmdir**" or "**rm**" command. 🗑️
    
    The "**rmdir**" command is used specifically to remove empty directories. For example:
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689597656866/293bf020-44a4-4908-9204-20717024cc8c.png align="center")
    
5. ## To create a fruits.txt file and to view the content.
    

To create a file in Linux, you can use the "**touch**" command.

For example:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689597819394/6b183f8a-0287-4587-92a5-40be53c4e68d.png align="center")

touch command will create a empty file.

To view the content of file you can use **cat** command.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689597951071/c276a2c1-724a-4fae-aa0b-bef29552ebc1.png align="center")

Nothing will be shown as it is empty file.

1. ## **Add content in fruits.txt (One in each line) - Apple, Mango, Banana, Cherry, Kiwi, Orange, Guava🍏🍇🍌🍒🥝🍊🍈**
    
    To add content to the "fruits.txt" file, you can use a **text editor** or the "**echo**" command to append each fruit on a new line. Here's an example using the text editor "vim":
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689601497193/64dff4ad-67d0-4fdc-8944-6dc01acba100.png align="center")
    
    ```plaintext
    vim fruits.txt
    ```
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689601460212/a328013d-0e0f-4313-9962-8c39cf17cd8c.png align="center")
    
    When you type command vim editor will open. Enter all the fruits name and then save. To save and exit esc+ !wq.
    
2. ## To Show only top three fruits from the file.
    
    To display only the top three fruits from the "fruits.txt" file, you can use the "**head**" command with the "**\-n**" option, specifying the number of lines you want to see. In this case, we want to see the first three lines, which represent the top three fruits in the file. 🍎🥭🍌
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689601740314/ca6eb898-9d39-485f-9ea3-0e4d2fd65319.png align="center")
    
3. ## To Show only bottom three fruits from the file.
    
    To display only the bottom three fruits from the "fruits.txt" file, you can use the "tail" command with the "-n" option, specifying the number of lines you want to see from the end of the file. In this case, we want to see the last three lines, which represent the bottom three fruits in the file. 🥝🍊🍏
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689601836088/d30eefc8-8a7b-4a37-a48a-419cddc5570e.png align="center")
    
4. ## To create another file Colors.txt and to view the content.
    
    To create a new file called "Colors.txt" in Linux, you can use the "touch" command followed by the desired filename. This command will create an empty file named "Colors.txt" in the current directory. Now, to view the content of the file, you can use the "cat" command:
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689602008046/de76e7f1-d04d-4937-aa75-d14243b15d95.png align="center")
    
5. ## Add content in Colors.txt (One in each line) - Red, Pink, White, Black, Blue, Orange, Purple, Grey.
    
    We can use **vim** editor or **echo** command.
    
    This time we'll use echo command.To add the specified content to the "Colors.txt" file with each color on a separate line, you can use the following command:
    

```plaintext
echo -e "Red\nPink\nWhite\nBlack\nBlue\nOrange\nPurple\nGrey" > colors.txt
```

If you view the content of the file using the `cat` command:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689602333652/e1d49ade-ebbb-43b4-b645-6315b86d795d.png align="center")

1. ## To find the difference between fruits.txt and Colors.txt file.
    
    To find the difference between the contents of two files, such as "fruits.txt" and "Colors.txt," you can use the "**diff"** command. Here's an example:
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689602480315/5356f1a7-18a2-4960-90df-490b4bc41edb.png align="center")
    
    ```plaintext
    diff fruits.txt colors.txt
    ```
    
    This command will compare the contents of "fruits.txt" and "Colors.txt" files. If there are any differences between the two files, the `diff` command will show them in the output.
    
    With the `diff` command, you can easily spot the variations between two files and manage your data more efficiently
    

# **Conclusion 🎉**

🎉🚀 Congratulations on mastering essential Linux commands! 📜💻 You've gained valuable skills in file interactions, permissions, and command analysis. From creating files to exploring their contents, you've become proficient in various Linux aspects. 📄📁 By using commands like "ls," "chmod," and "rm," you're now a Linux command-line pro! "Less" and "more" help you read files effortlessly. 📝👓 You've even created "fruits.txt" and "Colors.txt" and learned to display top and bottom items with "head" and "tail." The "diff" command aids in identifying file differences. 🍏🍇🍒 Keep practicing and exploring as your Linux adventure thrives! 💪💡 Embrace the command line's power and discover new possibilities in the vast Linux world. 🌐🐧 Happy DevOps exploring! 🌟🚀🔧

Stay in the loop with my latest insights and articles on cloud ☁️ and DevOps 🚀 by following me on Hashnode, LinkedIn ([**www.linkedin.com/in/Divyansh-Jain**](http://www.linkedin.com/in/divyansh-jain-03496617a/)), and GitHub ([**https://github.com/Divyansh-jain**](https://github.com/Divyanshji)).

**Thank you for reading!** 🙏 Your support means the world to me. Let's keep learning, growing, and making a positive impact in the tech world together.