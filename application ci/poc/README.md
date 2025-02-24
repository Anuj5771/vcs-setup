# Proof of Concept: FOSSA

| **Author** | **Created on** | **Version** | **Last updated by**|**Internal Reviewer** |**Reviewer L0** |**Reviewer L1** |**Reviewer L2** |
|------------|---------------------------|-------------|---------------------|-------------|-------------|-------------|-------------|
| Anuj yadav|   24-02-2025             | v1.1          | Anuj yadav     |  Siddharth pawar | Tarun Singh  | Abhishek  | Abhishek Dubey|     

![image](https://github.com/user-attachments/assets/341af05f-117e-4430-90ec-704a4f3e3987)

# FOSSA Integration Setup

## Pre-requisites

Before getting started, make sure you have the following:

1. **Access to FOSSA**: 
   - Sign up for a FOSSA account if you don’t already have one.
   - Ensure you have access to the FOSSA dashboard.
   - Get your FOSSA API token for configuration.

2. **Project Repository**: 
   - Make sure your project’s source code is hosted on a supported version control system (such as GitHub, GitLab, Bitbucket, etc.).

3. **System Requirements**: 
   - Ensure that you have internet access from your development environment.
   - Make sure your system meets the necessary specifications to run FOSSA CLI.

---

## Setup and Configuration

Follow these steps to install and configure FOSSA CLI:

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
## Integrate License Scanning in the Project

### Initialize FOSSA in the Project:
Navigate to the project directory and initialize FOSSA by running:

```bash
fossa init
```

## Run FOSSA Analysis Locally

Execute the CLI to analyze your project dependencies:

```bash
fossa analyze
```
- eview the analysis results in your terminal or the FOSSA dashboard.
![image](https://github.com/user-attachments/assets/05927c86-cade-447f-80da-db355718632e)

![image](https://github.com/user-attachments/assets/e84ab416-3cfd-43b1-b446-3f6fa6abfc8c)

