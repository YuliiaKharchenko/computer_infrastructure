# The module "Computer Infrastructure" 

![Image_computers](https://upload.wikimedia.org/wikipedia/commons/thumb/8/88/Laplacescher_D%C3%A4mon_%28Weltzentrale%29.jpg/640px-Laplacescher_D%C3%A4mon_%28Weltzentrale%29.jpg)



***

# Repository Files Description

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

### **1. Prerequisites**
- Install Git on your local machine.
- If analyzing weather data in Python, ensure you have Python 3 installed along with the required packages (`pandas`, etc.). Use `pip install -r requirements.txt` to set up dependencies.

### **2. Setup**
1. Clone the repository:  
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
   cd YOUR_REPOSITORY
   ```
***

## Usage Guide

### **For Daily Automation**
The repository includes a GitHub Actions workflow to automate the script execution and data updates.
To enable this:
Push all changes to GitHub.
Ensure the GitHub Actions workflow is set up in .github/workflows/weather-data.yml.
Check GitHub Actions logs for successful runs.

### **For Data Analysis**
Open the Jupyter Notebook (weather.ipynb) to explore the weather data and learn how it can be processed using Python.

## Author

Created by **Yuliia Kharchenko**. 

***

#### END