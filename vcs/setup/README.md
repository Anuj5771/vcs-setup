# POC of GitHub Setup

| **Author** | **Created on** | **Version** | **Last updated by**|**Last Edited On**|**Level** |**Reviewer** |
|------------|---------------------------|-------------|----------------|-----|-------------|-------------|
|Anuj Yadav|  24-02-2025              | v2          | Sharvari Khamkar |20-02-2025    | L2 |  Abhishek |
|Anuj Yadav|               | v2          | Sharvari Khamkar |19-02-2025    | L1 |  Taranddeep |
|AnujYadav|                | v2          |Sharvari Khamkar |19-02-2025    |  L0 | Akshit kapil | 
|AnujYadav|                | v1          | Sharvari Khamkar  |19-02-2025    |  Internal Reviewer | Komal Jaiswal |

## **Table of Contents**  

<details>  
  <summary>Sign Up for GitHub</summary>  

- [Create a GitHub Account](#create-a-github-account)  
- [Verify Email Address](#verify-email-address)   

</details>  

<details>  
  <summary>Git Installation</summary>  

- [Install Git on Windows](#install-git-on-windows)  
- [Install Git on Linux](#install-git-on-linux)  
- [Install Git on Mac OS](#install-git-on-mac-os)  
- [Check Git Version](#check-git-version)  

</details>  

<details>  
  <summary>Configure Git</summary>  

- [Set User Name and Email](#set-user-name-and-email)  
- [Check for an Existing SSH Key](#check-for-an-existing-ssh-key)  
- [Generate a New SSH Key](#generate-a-new-ssh-key)  
- [Copy the SSH Key](#copy-the-ssh-key)  
- [Add the SSH Key to GitHub](#add-the-ssh-key-to-github)
- [Generate a GitHub Personal Access Token](#generate-a-github-personal-access-token)  
- [Use the Token for Authentication](#use-the-token-for-authentication)

</details>  

<details>  
  <summary>Clone a Repository</summary>  

- [Copy Repository URL](#copy-repository-url)  
- [Clone the Repository](#clone-the-repository)  

</details>  

---  

## **Sign Up for GitHub**  

### Create a GitHub Account  
1. Go to [GitHub](https://github.com/).
![Screenshot 2025-02-20 132620](https://github.com/user-attachments/assets/55ed579b-e352-416a-afbc-14f3a474ecb4)

2. Click **Sign up** and enter your details (username, email, password).
![Screenshot 2025-02-20 132852](https://github.com/user-attachments/assets/4b17018b-73d4-4b8b-b5ae-72a2d674ad6f)

### Verify Email Address
3. Complete the verification process and click **Create account**.
![Screenshot 2025-02-20 133054](https://github.com/user-attachments/assets/721ec315-f9f6-498b-87f9-802d07569104)
![Screenshot 2025-02-20 133019](https://github.com/user-attachments/assets/a8d247e2-9300-441d-82fa-fa73bb2c09b8)
![Screenshot 2025-02-20 133437](https://github.com/user-attachments/assets/65adfa1c-2d08-456e-a1fe-b99ef6362c04)

## **Install Git**  

### Install Git on Windows  
1. Download Git for Windows from [Git for Windows](https://gitforwindows.org/).
2. Run the installer and follow the setup instructions.
3. Choose the default options unless you need specific configurations.
4. Finish installation and open **Git Bash** to verify installation.

### Install Git on Linux  
Run the following command based on your Linux distribution:

#### Ubuntu/Debian  
```sh
sudo apt update && sudo apt install git -y
```

#### CentOS/RHEL  
```sh
sudo yum install git -y
```

#### Fedora  
```sh
sudo dnf install git -y
```

### Install Git on Mac OS  
1. Install Homebrew if not already installed:
```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
2. Install Git using Homebrew:
```sh
brew install git
```

## **Check Git Version**  
Verify the installation by checking the Git version:  
```sh
git --version
```

## **Configure Git**  

Before configuring Git locally, ensure you have a GitHub account.  

### Set User Name and Email  
Set your Git user name and email address, which will be associated with your commits:  
```sh
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

### Check for an Existing SSH Key  
Navigate to the `~/.ssh` directory to check if a public key already exists.  

If there's no public key, create a new one.  

### Generate a New SSH Key  
Run the following command to generate an SSH key:  
```sh
ssh-keygen
```

### Copy the SSH Key  
Copy the generated SSH key to add it to GitHub.  

### Add the SSH Key to GitHub  
1. Go to your GitHub account settings.  
2. Click on **SSH and GPG keys**.  
3. Click **New SSH Key**.  
4. Add a title and paste the copied key into the key box.  
5. Click **Add SSH Key**.  

## **Configure Git using Token Setup**  

### Generate a GitHub Personal Access Token  
1. Go to **GitHub → Settings**.  
2. Navigate to **Developer Settings → Personal Access Tokens**.  
3. Click **Generate new token (classic)**.  
4. Select the necessary scopes (repo, workflow, admin:repo_hook, etc.).  
5. Click **Generate token** and copy it securely.  

### Use the Token for Authentication  

#### Using Git CLI  
Use the token in place of your password when prompted:  
```sh
git clone https://<github-username>@github.com/<repository>.git
Username: <your-github-username>
Password: <your-generated-token>
```

#### Storing the Token Securely  
To store the token for future use:  
```sh
git config --global credential.helper store
```
Now, when prompted, enter your token once, and it will be stored securely.

## **Clone a Repository**  

To clone a repository from GitHub:  

### Copy Repository URL  
1. Go to the GitHub repository you want to clone.  
2. Click **Code → Select SSH** → Copy the URL.

### Clone the Repository  
Run the following command to clone the repository to your local system:  
```sh
git clone <repository-url>
```

# Contact Information  

| **Name**    | **Email address**         |
|-------------|---------------------------|
| Sharvari Khamkar | sharvari.khamkar@mygurukulam.co   |

# References  

| **Link** | **Description** |
|----------------------------------------------------|--------------------|
| [Conclusion Docs](https://github.com/snaatak-Zero-Downtime-Crew/Documentation/blob/Mohit-SCRUM-23/VCS/Features%20of%20VCS/Conclusion/README.md) | Why we choose GitHub ? |
