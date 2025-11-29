# Employee Data Analysis Project

## 📌 Project Overview
This project undertakes a comprehensive analysis of employee data to gain insights into workforce dynamics, with a particular emphasis on **employee attrition and turnover rates**. By scrutinizing various factors such as job titles, pay zones, business units, and performance scores, this analysis seeks to uncover underlying patterns and pinpoint areas for strategic improvement within human resource management.

## 🎯 Objectives
*   **Calculate Tenure**: Determine the length of service for each employee.
*   **Identify Attrition**: Accurately flag employees who have left the organization.
*   **Analyze Turnover Rates**: Calculate and visualize turnover rates across different dimensions (Department, Job Title, Pay Zone, Business Unit).
*   **Data Visualization**: Provide clear visual representations of the workforce status and attrition drivers.

## 📂 Repository Structure
*   `Employee_Data_Analysis.ipynb`: The main Jupyter Notebook containing the data loading, cleaning, analysis, and visualization code.
*   `Employee Data.xlsx`: The source dataset containing employee records.
*   `Business Problem for HR Analyst.pdf`: Contextual document outlining the business problem.
*   `hr_analysis_outputs/`: Directory for generated output files (e.g., `supervisor_turnover_sample.csv`).

## 📊 Key Analysis & Methodology

### 1. Data Preprocessing
*   **Column Normalization**: Standardized column names to handle variations (e.g., mapping `StartDate` to `HireDate`).
*   **Tenure Calculation**: Computed employee tenure in years based on `StartDate` and `ExitDate` (or current date for active employees).
*   **Exit Flagging**: Created a robust `exited` binary flag derived from `EmployeeStatus` and `ExitDate` to accurately identify turnover.

### 2. Exploratory Data Analysis (EDA)
*   **Overall Turnover**: Calculated the organization-wide turnover rate.
*   **Segmented Analysis**: Broken down turnover rates by:
    *   **Job Title**: Identifying high-risk roles (e.g., Data Architect, Enterprise Architect).
    *   **Pay Zone**: Analyzing if compensation tiers impact retention (e.g., Zone B vs. Zone A).
    *   **Business Unit**: Comparing performance across different business divisions.
    *   **Department**: Evaluating departmental retention health.

## 🚀 How to Run
1.  Ensure all required libraries are installed:
    ```bash
    pip install pandas numpy matplotlib seaborn openpyxl
    ```
2.  Open `Employee_Data_Analysis.ipynb` in Jupyter Notebook or JupyterLab.
3.  Run all cells to execute the analysis and generate visualizations.

## 📈 Sample Insights
*   **High Turnover Roles**: Preliminary analysis suggests significantly higher turnover in specific technical roles like "Data Architect".
*   **Pay Zone Impact**: "Zone B" appears to have a higher turnover rate compared to other zones, suggesting potential compensation alignment issues.