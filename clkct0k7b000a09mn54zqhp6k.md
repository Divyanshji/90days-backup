---
title: "Understanding package manager and systemctl"
datePublished: Fri Jul 21 2023 16:37:01 GMT+0000 (Coordinated Universal Time)
cuid: clkct0k7b000a09mn54zqhp6k
slug: understanding-package-manager-and-systemctl
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1689957376736/4c8cbcbe-a05e-4c4a-99dd-27131742be4e.png
tags: linux, devops, 90daysofdevops, day7, divyanshjain

---

## Introduction

Hello, fellow technology nerds! We're delving into the fascinating realm of Linux package management today. Understanding package managers may significantly improve your experience and increase your productivity, whether you are an experienced Linux user or are just beginning your adventure. So let's start this thrilling journey!

## What is Package manager in Linux?

A package manager is a software tool used to automate the process of installing, upgrading, configuring, and removing software packages in a Linux-based operating system. It acts as a central repository that contains pre-compiled software packages along with metadata, such as package descriptions, version numbers, and dependencies.

## Types of Package Managers

There are several package managers used in various Linux distributions. Some of the most common ones include:

1. **APT (Advanced Package Tool)** - Used in Debian and Ubuntu-based systems.
    
2. **YUM (Yellowdog Updater Modified)** - Found in Red Hat, CentOS, and Fedora-based systems.
    
3. **DNF (Dandified YUM)** - The next-generation package manager for Fedora and other RPM-based distributions.
    
4. **Dpkg(Debian Package Management System) -** This is a base package management system for the Debian Linux family, it is used to install, remove, store, and provide information about `.deb` packages.
    

**RPM (Red Hat Package Manager) -** This is the Linux Standard Base packing format and a base package management system created by RedHat.

## **Installation of Docker on Ubuntu**

**Preparing the Environment:** Before we begin, ensure your Linux system is up-to-date with the latest packages and dependencies. Open a terminal and run the following commands:

```plaintext
sudo apt-get update
```

Install **Docker** using the following command:

```plaintext
 sudo apt install docker.io -y
```

Install all the dependency packages using the following command:

```plaintext
 sudo apt install snapd -y

 sudo snap install docker
```

  
Before testing Docker, check the version installed using the following command:

```plaintext
 docker --version
```

**Start and Enable Docker Service:**

Once Docker is installed, start and enable the Docker service to run on system boot.

```plaintext
sudo systemctl start docker 
sudo systemctl enable docker
```

Use this command to check status of docker:

```plaintext
sudo systemctl status docker
```

# **Installation of Jenkins on Ubuntu**

Installation of Java as per the prerequisite

```plaintext
 sudo apt-get install openjdk-11-jdk -y
```

Adding the repository to the system

```plaintext
 curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee \
   /usr/share/keyrings/jenkins-keyring.asc > /dev/null
 echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
   https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
   /etc/apt/sources.list.d/jenkins.list > /dev/null
```

After both commands have been entered, run apt update so that apt will use the new repository.

```plaintext
 sudo apt-get update
```

Finally, install Jenkins and check the status:

```plaintext
 sudo apt-get install jenkins
```

```plaintext
 sudo systemctl status jenkins
```

## systemctl & systemd

Systemd is a system and service manager for Linux operating systems. It is responsible for starting and stopping system services and managing system resources. Systemd was introduced as a replacement for the traditional SysVinit system initialization process and has become the standard for many modern Linux distributions.

Systemctl is a command-line tool that is part of the systemd suite of tools. It is used to control and manage services that are managed by systemd. With systemctl, you can start, stop, restart, enable, and disable services, as well as view the status of running services and get information about services that are installed on your system.

**Checking Docker Service Status**

To check the status of Docker service, simply enter the following command:

```plaintext
systemctl status docker
```

**Stopping Jenkins Service**

Let's put Jenkins on pause for a moment. Use the following commands to stop the Jenkins service:

```plaintext
sudo systemctl stop jenkins
```

**Before and After Screenshots**

Take screenshots before stopping the Jenkins service and after stopping it, and witness the magical change! ✨

## systemctl vs service

Systemctl is the newer command for systems that boot with systemd instead of init. Systemctl is a combination of service and chkconfig for those newer systems. If you accidentally use a service on a systemd-based system, the arguments will be swapped (ie: service httpd restart will become systemctl restart httpd). They serve the same function, but they interact with different systems.

“Service” is the legacy command, which normally works with classical init. Although on systems which use systemd it’s actually more of a wrapper over the actual systemd native means of managing services, namely systemctl.

You use service on init systems other than systemd. You use systemctl on systemd.

To check the Docker status, use:

```plaintext
systemctl status docker
```

Or

```plaintext
service docker status
```

## Conclusion

Package managers in Linux are indispensable tools for DevOps engineers, offering streamlined software management, dependency resolution, version control, and security updates. By leveraging these powerful tools, DevOps professionals can focus on delivering robust applications and services while maintaining a stable and secure infrastructure. Understanding how package managers work and mastering their usage will undoubtedly contribute to a more efficient and seamless software deployment process in the Linux ecosystem.

Stay in the loop with my latest insights and articles on cloud ☁️ and DevOps 🚀 by following me on Hashnode, LinkedIn ([**www.linkedin.com/in/Divyansh-Jain**](http://www.linkedin.com/in/divyansh-jain-03496617a/)), and GitHub ([**https://github.com/Divyansh-jain**](https://github.com/Divyanshji)).

**Thank you for reading!** 🙏 Your support means the world to me. Let's keep learning, growing, and making a positive impact in the tech world together.