# VCS GitHub Setup POC

# Table of Contents
- [Purpose](#purpose)
- [Pre-requisites](#pre-requisites)
- [System Requirements](#system-requirements)
- [Dependencies](#dependencies)
- [Architecture](#architecture)
- [Step-by-step installation of GitHub](#step-by-step-installation-of-github)
- [Conclusion](#conclusion)
- [Contact Information](#contact-information)
- [References](#references)

## Purpose

This POC shows how to set up and use GitHub as a Version Control System (VCS). GitHub is a platform that helps teams work together on software projects. It provides tools like version control, issue tracking, and project management to make collaboration easier.

## Pre-requisites
- Basic understanding of Git and version control concepts.
- A GitHub account.

## System Requirements

### Hardware Specifications
| Component | Minimum | Recommended |
|-----------|---------|-------------|
| **RAM**   | 1 GB    | 4 GB or more|
| **Disk**  | 8 GB free space | 20 GB free space |
| **OS**    | Windows 10, macOS 10.14, Ubuntu 18.04 or later | Latest stable version of your preferred OS |


## Dependencies

| Name | Version | Description                           |
|------|---------|---------------------------------------|
| Git  | 2.34    | Distributed version control system    |


## Architecture

![image](https://github.com/user-attachments/assets/d9d3717a-1f72-4c63-8a1a-cecda88cec06)


## Step-by-step installation of GitHub

### Install Git:

- **Windows (using Chocolatey):**
  ```bash
  choco install git

- **macOS (using Homebrew):**
  ```bash
  brew install git
  ```
- **Ubuntu**
  ```bash
  sudo apt-get update
  sudo apt-get install git
  ```

## Create a GitHub Account and Repository

### 1. Create a GitHub account
- Go to [github.com]() and sign up for a new account.

### 2. Create a new repository on GitHub:
- Click the "+ or add new" icon in the top-right corner.
- Select **New repository**.
- Name your repository.
- Choose **Private** if you want to keep the repository private.
- Click **Create repository**.



## Set up Local Repository

1. **Create a new directory for your repository**:
  
```bash
mkdir vcs-setup-repo
cd vcs-setup-repo/
echo "# vcs-setup-poc-" >> README.md
git init
git add README.md
git status
git commit -m "this is my first vcs setup"
git branch -M main
git remote add origin https://github.com/devneelesh921/vcs-setup-poc-.git
git push -u origin main
cd .ssh
cat id_rsa.pub
git remote add sshorigin git@github.com:devneelesh921/vcs-setup-poc-.git
git push sshorigin main
```


## Conclusion

In this Proof of Concept (PoC), we demonstrated the basic process of creating a repository, cloning it, and pushing changes. This workflow allows developers to track modifications, collaborate smoothly, and ensure an organized approach to managing project files and updates. By following these steps, teams can streamline their development efforts and enhance productivity across the board.

## Contacts

| Name            | Email Address                                |
|-----------------|----------------------------------------------|
| Anuj Yadav   | [) |
| anuj5771921   | [() |

## References

| Links                                                                                       | Description     |
|---------------------------------------------------------------------------------------------|-----------------|
| [Introduction to Bitbucket](https://www.geeksforgeeks.org/introduction-to-bitbucket/?ref=ml_lbp) | For Bitbucket   |
| [Introduction to GitHub](https://www.geeksforgeeks.org/introduction-to-github/?ref=ml_lbp)     | For GitHub      |
| [GitLab Introduction](https://www.tutorialspoint.com/gitlab/gitlab_introduction.htm)           | For GitLab      |
