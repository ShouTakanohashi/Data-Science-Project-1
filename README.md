# README
Shou Taknohashi

## Table of Contents

- [1. Purpose of the Project](#1-purpose-of-the-project)
- [2. Overview of workflow](#2-overview-of-workflow)
- [3. Setting Up the Development Environment](#3-setting-up-the-development-environment)
    - [3.1 Tools Used](#31-tools-used)
    - [3.2 Steps Taken to Set Up the Environment](#32-steps-taken-to-set-up-the-environment)
- [4. Phases After Setting Up the Environment](#4-phases-after-setting-up-the-environment)
- [5. File Structure](#5-file-structure)


## 1. **Purpose of the Project**
This is my first project, which demonstrates the full steup of a data sceience development environment and lays the groudndwork for long-term analytical projects.

## 2. Literature review

We first focus on understanding carbon credits and carbon trading systems and analyze the existing work.

1. **Definition and history of carbon credit**



Carbon credits have two main types:
    1. Voluntary emissions reduction (VER)
        - Carbon offset that is exchanged in voluntary market for credits. No third party certifying body.
    2. Certified emissions reduction (CER)
        - Emission units are created through a regulatory framework with the purpose of offsetting a project's emission. There are third party bodies that certifying credits.



2. **Carbon trade**


3. 


4. **Effectiveness**



## 3. Setting Up the Development Environment

### 3.1 Tools Used
This project is built with setup as following:
- Operating System: Ubuntu (via Windows Subsystem for Linux)
- Package and environment manager: Miniconda
- Language: Python 3.11
- Editor: Visual Studio Code
- Version Control: Git and GitHub (via SSH)
- Key extensions in VS Code:
    - Python
    - Jupyter
    - GitLens
    - WSL

### 3.2 Steps Taken to Set Up the Environment
1. Installed Ubuntu via Windows Subsystem for Linux (WSL)
2. Installed Miniconda inside Ubuntu
3. Created a conda virtual environment
4. Installed Python packages, including:
    - ipkernel
    - jupyter
    - pandas
5. Registered the environment for use in VS Code 
6. Generated an SSH key and added it to GitHub for secure authentication
7. Installed VS Code and necessary extensions listed above
8. Opened the Ubuntu terminal in VS Code via Ctrl + Shift + P and "WSL: Connect to WSL"
9. Cponed the GitHub repository from inside the Ubuntu file system
10. Activated the virtual environment
11. Selected the correct kernel in VS for .ipynb notebook execution

## 4. Phases After Setting Up the Environment
1. Dataset acquisition and import
2. Initial cleaning and validation
3. Exploratory Data Analysis (EDA)
4. Visualizations
5. Insights
6. Documentation and packaging for portfolio


1. Dataset acquisition and import



2. Initial cleaning and validation

    1. First, we need to check for data types in each column and look for missing values.
    2. We convert `Estimated Annual Emission Reduciton` column data type from object to integer.
    3. We convert `Project Registration Date`, `Crediting Period Start Date`, and `Crediting Period End Date` into datatime type.
    4. We standardize and encode `Project Type`, `AFOLU Activities`, `Status`, and `Region`.
        1. We fill or drop missing values where appropriate.
            - i.e., if `Region` is missing but `Country` is available, we may consider imputing region manually.
    5. We may perform feature engineering when appropriate. For example:
        1. Project duration: in years or months.
        2. Normalized emission reduciton: per year, or per project type.
        3. Category binning: group smaer countries or activity types into "Other."


3. Exploratory Dadta Analysis (EDA)



4. Visualizations

## 5 Findings


## 6. Limitations.
While this project analyzes publicly available data on carbon credit projects, it is important to recognize the ongoing debates surrounding the carbon credit market itself. Some argue that many credits, especially avoidance-based ones, do not represent additional or durable carbon reducitons and may contribute to greenwashing.

This proejct does not attempt to validate or discredit the carbon credit system as a whole. Instead, it focuses on comparing project types and analyzing regional distributions, while acknowledging that data availability, verification rigor, and market mechanisms vary significantly across projects.

## 7. Sources

https://interactive.carbonbrief.org/carbon-offsets-2023/timeline.html 

https://climateseed.com/blog/understanding-carbon-credits 

https://bezerocarbon.com/ 

https://www.ceezer.earth/insights/risk-impact-carbon-market#:~:text=BeZero%20Carbon%20is%20a%20carbon,a%20growing%20number%20of%20projects.

https://carboncredits.com/what-is-the-voluntary-carbon-market/ 

https://carboncredits.com/how-to-invest-in-carbon-credits-carbon-etfs-and-carbon-stocks/ 

https://www.nature.com/articles/s41597-022-01659-x

