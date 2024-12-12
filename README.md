# Computer Infrastructure

![Image_computers](https://upload.wikimedia.org/wikipedia/commons/thumb/8/88/Laplacescher_D%C3%A4mon_%28Weltzentrale%29.jpg/640px-Laplacescher_D%C3%A4mon_%28Weltzentrale%29.jpg)

This repository contains all my work on the **Computer Infrastructure** module of the [ATU](https://www.atu.ie/) **Higher Diploma in Science in Computing in Data Analytics** course. The repository includes a series of module tasks as well as project implementation. 
The description of the series of tasks and the project are given [here](https://github.com/ianmcloughlin/2425_computer_infrastructure?tab=readme-ov-file#repository-20).

***

## Work Environment: GitHub Codespaces

All the work for this module was conducted using **GitHub Codespaces**, a cloud-based development environment provided by GitHub. It eliminates the need for local setup and offers a fully configured workspace accessible from any device with internet access.
**GitHub Codespaces** operates on a **Linux-based infrastructure**, providing a robust, consistent, and flexible environment for software development. Leveraging the power of Linux containers, Codespaces ensures compatibility with a wide range of tools, frameworks, and workflows.

### Advantages of GitHub Codespaces 

1. **No Local Setup Required**: You don't need to install tools like Git, Python, or other dependencies on your local machine.
2. **Consistency Across Environments**: Ensures a standardized development environment for all contributors.
3. **Instant Access to Tools**: Comes preloaded with Git, Docker, and editors like VS Code.
4. **Flexibility**: Accessible from any device via browser or VS Code.
5. **Integrated with GitHub**: Simplifies workflows like cloning, committing, and pushing to repositories.

### How It Was Used in This Module

1. **Repository Management**: Codespaces was used to clone the repository, manage files, and commit changes directly to GitHub.
2. **Script Execution**: Bash scripts, such as `weather.sh`, were executed in the Codespaces terminal to automate tasks like downloading weather data.
3. **Notebook Editing**: The `weather.ipynb` notebook was created and edited within Codespaces to analyze and summarize the collected data.
4. **Workflow Testing**: GitHub Actions workflows were tested and debugged in this cloud environment.

***

## Repository Files Description

1. **.github/workflows**  
> **File format:** Directory  
> **Description:**  Contains the GitHub Actions workflow `weather-data.yml`, which automates the execution of the `weather.sh` script daily, fetches weather data, and commits it back to the repository.

2. **data/**  
> **File format:** Directory  
> **Description:** 
> - **data/timestamps**: Stores files containing timestamp data in raw and formatted forms.  
> - **data/weather**: Contains weather data in JSON format fetched from the Met Éireann API.

3. **img/**  
> **File format:** Directory  
> **Description:** Placeholder for any images used in documantation or reports.

4. **.gitignore**  
> **File format:** Text  
> **Description:** Specifies files and directories for Git to ignore during commits and updates, ensuring unnecessary or temporary files are excluded.

5. **README.md**  
> **File format:** Markdown  
> **Description:** Provides an overview of the repository, its purpose, and instructions for usage.

6. **requirements.txt**  
> **File format:** Text  
> **Description:** Lists Python dependencies for analyzing weather data using tools like `pandas`.

7. **weather.ipynb**  
> **File format:** Jupyter Notebook  
> **Description:**  
Contains the report documenting how tasks (1–7) were completed and demonstrates the analysis of weather data using the `pandas` library.

8. **weather.sh**  
> **File format:** Shell Script  
> **Description:** Automates the process of downloading and timestamping weather data, saving it to the appropriate directory.

## Getting Started

You can work on this project either **locally on your computer** or using **GitHub Codespaces**

### **1. Using GitHub Codespaces**

1. **Starting Codespaces**:
   - Navigate to your repository page on GitHub.
   - Click the `Code` button and select the `Codespaces` tab.
   - Create a new Codespace or select an existing one.

2. **Development Environment**:
   - Codespaces comes pre-installed with all necessary tools like Git, Bash, and Python.
   - To install dependencies, run:
     ```bash
     pip install -r requirements.txt
     ```

3. **Benefits of Codespaces**:
   - No need to set up a local environment.
   - Runs on a stable Linux platform.
   - Fully integrated with GitHub for automation and version control.

---

### **2. Local Development**
If you prefer to work locally, ensure your machine runs a Linux operating system or has a Linux-like environment set up (e.g., macOS or Windows with WSL). Follow these steps:

1. **Install Required Tools**:
   - Install [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) on your local machine.
   - Ensure [Python 3](https://www.python.org/downloads/) is installed.
   - Install dependencies using:
     ```bash
     pip install -r requirements.txt
     ```

2. **Clone the Repository**:
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
   cd YOUR_REPOSITORY

3. **Set Up Your Local Environment**:
   - Ensure Linux-native commands like `wget`, `bash`, `touch`, and `date` are available on your system.
   - Configure scripts and perform tests to ensure functionality.

***

## Usage Guide

### **For Daily Automation**
The repository includes a GitHub Actions workflow to automate the execution of the weather script and the updating of weather data in the repository.

To enable this automation:
1. Push all changes to GitHub.
2. Ensure that the GitHub Actions workflow is correctly configured in `.github/workflows/weather-data.yml`.
3. Monitor the workflow execution by checking the logs in the "Actions" tab of your GitHub repository to verify successful runs.

### **For Data Analysis**
To analyze the downloaded weather data:
1. Open the Jupyter Notebook (`weather.ipynb`) included in the repository.
2. Follow the step-by-step guidance in the notebook to process the weather data files using Python.
3. Use the provided `pandas` scripts to load, examine, and summarize the data.

### **Important Notes**
- **Environment Compatibility**: Ensure that the environment (GitHub Codespaces or local Linux) matches the setup steps outlined in the "Getting Started" section.
- **Data File Locations**: All weather data files are saved in the `data/weather/` directory, organized with timestamped filenames.

***

## Author

Created by **Yuliia Kharchenko**. 

***

#### END

***
