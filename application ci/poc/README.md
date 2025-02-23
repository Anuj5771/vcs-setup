# Proof of Concept: FOSSA

![image](https://github.com/user-attachments/assets/0124f761-2ad6-4c46-af30-2564596bb5e6)


| **Author** | **Created on** | **Version** | **Last updated by** | **Internal Reviewer** | **Reviewer L0** | **Reviewer L1** | **Reviewer L2** |
|------------|--------------|-------------|----------------|-----------------|-------------|-------------|-------------|
| Anuj Yadav | 24-02-2025   | v1.1        | Anuj Yadav     | Siddharth Pawar | Tarun Singh | Abhishek    | Abhishek Dubey |

## Table of Contents
1. [Clone the Repository and Navigate to the Project Directory](#clone-the-repository-and-navigate-to-the-project-directory)
2. [Setup and Configuration](#setup-and-configuration)
   - [Install FOSSA CLI](#install-fossa-cli)
   - [Authenticate the FOSSA CLI](#authenticate-the-fossa-cli)
3. [Integrate License Scanning in the Project](#integrate-license-scanning-in-the-project)
4. [Run FOSSA Analysis Locally](#run-fossa-analysis-locally)

## Clone the Repository and Navigate to the Project Directory

```bash
git clone https://github.com/snaatak-Zero-Downtime-Crew/attendance-api.git
cd attendance-api
```


## Setup and Configuration

### Install and Verify FOSSA CLI Installation

To install the FOSSA CLI globally using npm:

```bash
npm install -g fossa-cli
fossa --version
```

- The installed FOSSA CLI version is 3.10.0 (revision 494e2795cf9f, compiled with GHC 9.8).

### Authenticate the FOSSA CLI

#### Obtain Your API Token
1. Go to the FOSSA dashboard.
2. Navigate to **Settings → API Keys**.
3. Generate or copy your API token.

#### Authenticate FOSSA CLI with Your API Token

Once you have the API token, run the following command to authenticate the FOSSA CLI:

```bash
fossa login --token <your-api-token>
```

### Initialize FOSSA in the Project

```bash
fossa init
```

This command initializes your project with FOSSA by setting up the necessary configuration files and preparing it for dependency and license analysis.

## Integrate License Scanning in the Project

To scan your project’s dependencies for license compliance, ensure your project is set up correctly and run:

```bash
fossa analyze
```

## Run FOSSA Analysis Locally

To verify your dependencies and licenses locally before pushing to the repository, execute:

```bash
fossa test
```

## Contact
| Name | Email Address | GitHub | URL |
|------|--------------|--------|-----|
| Anuj Yadav | anuj.yadav@mygurukulam.co | [anuj169](https://github.com/anuj169) | https://github.com/anuj169 |

---

