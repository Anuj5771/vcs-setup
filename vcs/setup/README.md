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
  ![image](https://github.com/user-attachments/assets/2cc8284b-5bdd-4995-94cd-04e66de25b36)

 ## Create a GitHub Account and Repository

 ### 1. Create a GitHub account
 - Go to [github.com]() and sign up for a new account.

 2. Create a new repository on GitHub:
 - Click the "+ or add new" icon in the top-right corner.
 - Select **New repository**.
 - Name your repository.
 - Choose **Private** if you want to keep the repository private.
 - Click **Create repository**.

 ![image](https://github.com/user-attachments/assets/56679ec3-f0ca-4e1a-94e0-1cc4ec0371b1)


 ### Generating a Personal Access Token (PAT) on GitHub

 Follow these steps to generate a Personal Access Token (PAT) on GitHub:

 1. **Go to GitHub Settings**
   - Navigate to [GitHub](https://github.com/) and click on your profile picture in the top right corner.
   - Select **Settings** from the dropdown menu.

2. **Navigate to Developer Settings**
   - Scroll down and click on **Developer settings**.
   - Under **Personal access tokens**, click on **Tokens (classic)**.

3. **Generate a New Token**
   - Click **Generate new token (classic)**.
   - Provide a **note** for the token (e.g., "My GitHub PAT").
   - Set an **expiration date** (or choose "No expiration" if preferred).

4. **Select Necessary Scopes**
    - Choose the required scopes based on your needs:
     - `repo` (Full control of private repositories)
     - `workflow` (Access to GitHub Actions workflows)
     - `admin:repo_hook` (Manage repository webhooks and services)
     - Other scopes as needed

5. **Generate and Copy the Token**
   - Click **Generate token**.
   - **Copy the token** immediately and store it securely (e.g., in a password manager).

- **Important:**
- Once you leave the page, you won't be able to see the token again.
- Do not share your token publicly or commit it to repositories.


![image](https://github.com/user-attachments/assets/ab8b66e5-39b8-4541-a54d-162ac40b018c)

![image](https://github.com/user-attachments/assets/1aeb2a91-ce21-42fa-9b42-546042292b69)

![image](https://github.com/user-attachments/assets/14756319-a3d0-4b7a-b96f-88affaf74cb3)

![image](https://github.com/user-attachments/assets/67d73aaa-6b05-4ccc-9077-0a7d6ccb02a1)

### Setting Up and Pushing First Commit to GitHub Repository
```bash
 mkdir vcs-setup-repo
 cd vcs-setup-repo/
 echo "# vcs-setup-poc-" >> README.md
 git init
 git add README.md 
 git status
 git commit -m "this is my first vcs setup"
 git branch -M main
 git remote add origin https://github.com/anuj169/Zero_Downtime_Crew.git
 git remote set-url origin https://<NEW_TOKEN>@github.com/anuj169/Zero_Downtime_Crew.git
 git add .
 git commit -m "update the file"
 git push origin main

```

## Conclusion

In this Proof of Concept (PoC), we demonstrated the basic process of creating a repository, cloning it, and pushing changes. This workflow allows developers to track modifications, collaborate smoothly, and ensure an organized approach to managing project files and updates. By following these steps, teams can streamline their development efforts and enhance productivity across the board.

## Contacts

## Contacts

| Name        | Email Address                               |
|-------------|---------------------------------------------|
| Anuj Yadav  | [anuj.yadav@mygurukulam.co](mailto:anuj.yadav@mygurukulam.co) |
| anuj169     | [https://github.com/anuj169) |


## References

| Links                                                                                       | Description     |
|---------------------------------------------------------------------------------------------|-----------------|
| [https://www.geeksforgeeks.org/introduction-to-bitbucket/?ref=ml_lbp#what-is-bitbucket) | For Bitbucket   |
| [https://www.geeksforgeeks.org/what-is-github-and-how-to-use-it/)     | For GitHub      |
