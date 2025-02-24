# Proof of Concept: FOSSA

| **Author** | **Created on** | **Version** | **Last updated by**|**Internal Reviewer** |**Reviewer L0** |**Reviewer L1** |**Reviewer L2** |
|------------|---------------------------|-------------|---------------------|-------------|-------------|-------------|-------------|
| Anuj yadav|   24-02-2025             | v1.1          | Anuj yadav     |  Siddharth pawar | Tarun Singh  | Abhishek  | Abhishek Dubey|     

# Table of Contents
1. [FOSSA Integration Setup](#fossa-integration-setup)
   - [Pre-requisites](#pre-requisites)
   - [System Requirements](#system-requirements)
2. [Setup and Configuration](#setup-and-configuration)
   - [Install FOSSA CLI](#install-fossa-cli)
   - [Authenticate the FOSSA CLI](#authenticate-the-fossa-cli)
3. [Integrate License Scanning in the Project](#integrate-license-scanning-in-the-project)
4. [Run FOSSA Analysis Locally](#run-fossa-analysis-locally)



## Clone the Repository and Navigate to the Project Directory

``bash
git clone https://github.com/snaatak-Zero-Downtime-Crew/attendance-api.git
cd attendance
```

## Installation and Setup

1. **Install FOSSA CLI**: 

   To install the FOSSA CLI, use npm to install it globally:

   ```bash
   npm install -g fossa-cli
  ```

![image](https://github.com/user-attachments/assets/2529a201-f218-414f-8ab8-82ebbe61686b)

# Authenticate the FOSSA CLI

## Obtain Your API Token:
1. Go to the FOSSA dashboard.
2. Navigate to **Settings → API Keys**.
3. Generate or copy your API token.

## Login to the CLI:
Once you have the API token, run the following command to authenticate the FOSSA CLI:

```bash
fossa login --token <your-api-token>
```

### Initialize FOSSA in the Project:

```bash
fossa init
```
- The fossa init command initializes your project with FOSSA by setting up the necessary configuration files and preparing it for dependency and license analysis.


## Run FOSSA Analysis Locally

Execute the CLI to analyze your project dependencies:

```bash
fossa analyze
```

- eview the analysis results in your terminal or the FOSSA dashboard.

![image](https://github.com/user-attachments/assets/05927c86-cade-447f-80da-db355718632e)

![image](https://github.com/user-attachments/assets/e84ab416-3cfd-43b1-b446-3f6fa6abfc8c)







 



