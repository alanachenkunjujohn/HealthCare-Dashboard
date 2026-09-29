# Healthcare Data Analysis and Interactive Dashboard

## Project Overview

The healthcare industry generates large volumes of data that can provide valuable insights into patient health, medical history, healthcare costs, and hospital services.

This project uses Microsoft Excel to clean, transform, analyse, and visualise healthcare data. By combining customer profiles, medical examination records, and hospitalisation details, the project aims to identify patterns in health conditions, lifestyle factors, hospital tiers, and healthcare charges.

The analysis is presented through charts, PivotTables, and an interactive dashboard to support data-driven insights.

## Project Objectives

* Clean missing and inconsistent values in healthcare datasets.
* Transform raw data into structured and meaningful information.
* Analyse BMI, HbA1C, smoking habits, cancer history, and major surgeries.
* Investigate relationships between patient age, health indicators, and healthcare charges.
* Compare healthcare costs across weight categories, diabetes statuses, states, and hospital tiers.
* Develop an interactive Excel dashboard with filters for Weight Status and Diabetes Status.

## Dataset Description

The project combines three datasets:

| Dataset                 | Description                                                                                       |
| ----------------------- | ------------------------------------------------------------------------------------------------- |
| Customer Names          | Customer identifiers and personal name information                                                |
| Medical Examinations    | BMI, HbA1C, heart issues, transplant history, cancer history, major surgeries, and smoking status |
| Hospitalisation Details | Date-related fields, healthcare charges, hospital tier, city tier, and state ID                   |

**Key field:** Customer ID is used to connect records across the three datasets.

## Tools and Technologies

* **Microsoft Excel** — data cleaning, transformation, analysis, and visualisation
* **Excel formulas** — missing-value handling, categorisation, date calculations, and VLOOKUP
* **PivotTables** — summarising and comparing healthcare data
* **PivotCharts** — visualising trends and relationships
* **Excel Slicers** — interactive filtering of dashboard visualisations

## Project Workflow

### 1. Data Cleaning

* Identified missing values represented by `?`.
* Replaced missing months with September.
* Replaced missing years with the rounded average year.
* Used the mode to fill missing smoking status, hospital tier, and city tier.
* Replaced missing State ID values with `Unknown`.
* Standardised categorical values where appropriate.

### 2. Data Transformation

* Split customer names into Title, First Name, and Last Name.
* Converted the NumberOfMajorSurgeries field into numeric values.
* Reviewed inconsistencies in Heart Issues and smoker fields.
* Categorised BMI into four weight-status groups:

  * Underweight
  * Normal Weight
  * Overweight
  * Obesity
* Categorised HbA1C into Normal, Prediabetes, and Diabetes.
* Combined year, month, and date into a Date of Birth field.
* Calculated customer age as of 8 June 2023.
* Formatted healthcare charges as currency.

### 3. Data Integration

Combined the three datasets into a consolidated Healthcare worksheet using Customer ID as the common identifier and VLOOKUP to retrieve corresponding fields.

The resulting dataset includes customer details, health indicators, medical history, age, healthcare charges, and hospital information.

### 4. Data Analysis and Visualisation

The analysis explores the following questions:

**Cancer History and Smoking**

* How does cancer history differ between smokers and non-smokers?

**Transplants and Medical History**

* How does the total number of major surgeries differ between patients with and without a history of transplants?
* How does average HbA1C compare between these groups?

**Healthcare Charges**

* How do average healthcare charges vary by weight status and diabetes status?
* How do average charges compare across hospital tiers within different states?

**Age and Health Indicators**

* Is there a relationship between age and BMI?
* Is there a relationship between age and HbA1C?
* How do healthcare charges vary with age?

Pie or doughnut charts, column charts, and scatter plots can be used to explore these questions.

### 5. Dashboard Development

The Excel dashboard brings together key metrics and visualisations to make the results easier to interpret.

Planned dashboard features include:

* Summary indicators for customer count, average age, BMI, HbA1C, and healthcare charges.
* Charts covering smoking, cancer history, transplants, medical indicators, and costs.
* Comparisons across weight status, diabetes status, states, and hospital tiers.
* Interactive slicers for Weight Status and Diabetes Status, connected to the relevant PivotTables.

## Workbook Structure

The Excel workbook contains the following worksheets:

| Worksheet               | Purpose                                     |
| ----------------------- | ------------------------------------------- |
| Customer Names          | Original customer information               |
| Medical Examinations    | Original medical examination data           |
| Hospitalisation Details | Original hospitalisation data               |
| Healthcare              | Consolidated and transformed dataset        |
| Data Quality            | Missing-value counts and cleaning decisions |
| Analysis                | Summary tables and charts                   |
| Dashboard               | Key insights and interactive visualisations |

## Key Skills Demonstrated

* Data cleaning and preprocessing
* Data transformation and categorisation
* Excel formulas and VLOOKUP
* Data integration using a common identifier
* PivotTables and PivotCharts
* Exploratory data analysis
* Data visualisation and dashboard design
* Analytical thinking and interpretation of healthcare data

## How to Use This Project

1. Download or clone this repository.
2. Open the Excel workbook in Microsoft Excel.
3. Review the source datasets and the Data Quality worksheet.
4. Explore the consolidated Healthcare worksheet.
5. Review the Analysis worksheet to examine summary tables and charts.
6. Open the Dashboard worksheet to explore the visualisations and, when configured, use the slicers to filter the results.

## Important Notes

* Age is calculated using 8 June 2023 as the reference date.
* Missing-value imputation and categorical classifications follow the project requirements.
* BMI and HbA1C categories are analytical groupings for this project and should not be treated as individual medical diagnoses.
* Findings describe patterns in the supplied dataset and do not establish causal relationships.
* The completeness and accuracy of results depend on the quality of the original data and the correctness of the cleaning process.

## Future Improvements

* Automate data cleaning and transformation using Python or Power Query.
* Add statistical correlation analysis and further exploratory analysis.
* Improve dashboard interactivity and usability.
* Extend the analysis to identify additional patterns in healthcare utilisation and costs.

## Conclusion

This project demonstrates how Microsoft Excel can be used to transform raw healthcare data into structured information, analyse relationships between health indicators and healthcare costs, and communicate findings through visualisations and dashboards.

The project highlights the role of data analysis in supporting evidence-based understanding of healthcare trends and resource utilisation.

---

**Project Category:** Data Analytics | Healthcare | Excel Dashboard

**Author:** Alan Achenkunju John

