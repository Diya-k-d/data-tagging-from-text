# Vehicle Service Data Analysis and Feature Tagging

## Description
This project focuses on data cleaning, exploratory data analysis (EDA), and feature generation from a dataset containing vehicle service and warranty records. The dataset includes both structured information (cost, vehicle details, repair information) and unstructured free-text fields describing customer complaints and technician corrections.

The objective of this project was to prepare the dataset for analysis, identify critical variables affecting failures and costs, generate meaningful tags from free text, and extract insights that could support better decision-making.

---

## Dataset Overview
The dataset contains information related to:

- Customer complaint descriptions
- Repair actions taken by technicians
- Failure-causing components
- Labor categories
- Repair costs
- Vehicle configuration details
- Dealer and regional information

Both structured and unstructured fields were analyzed to gain a comprehensive understanding of failure patterns and repair trends.

---

## Data Cleaning and Preparation
Several data quality issues were identified and resolved during preprocessing:

### Handling Missing Values
Missing values were handled using appropriate placeholders to maintain dataset consistency.

### Text Standardization
Text fields were standardized by removing extra spaces and correcting formatting inconsistencies to prevent duplicate category creation.

### Duplicate Removal
Duplicate records were identified and removed to avoid double counting.

### Numeric Formatting
Cost-related fields were converted to numeric format to ensure accurate calculations.

### Data Consistency
String values such as "Nan", "nan", and empty strings were converted into proper missing values and handled accordingly.

These steps ensured that the dataset was clean, structured, and ready for analysis.

---

## Critical Columns Identified
Based on analytical importance, the following fields were selected as the most critical for analysis:

1. Customer complaint description
2. Technician correction description
3. Component responsible for failure
4. Repair category
5. Total repair cost

These columns help answer key questions such as:

- What failed?
- Why did it fail?
- How was the issue fixed?
- Which components are responsible for failures?
- What is the financial impact of these failures?

---

## Exploratory Data Analysis
Exploratory analysis was performed to identify important patterns in the dataset.

Three key visualizations were created:

- Top failure-prone components
- Most common repair categories
- Components contributing the highest repair cost

Bar charts were used because they provide clear comparisons across categorical variables and help stakeholders quickly understand trends.

---

## Feature Tag Generation from Text
Meaningful tags were generated from free-text complaint descriptions using rule-based logic. Examples of generated tags include:

- Leak
- Sensor issue
- Noise issue
- Steering issue
- Transmission issue
- Overheating
- Vibration

These tags help summarize unstructured text data and enable faster analysis of common failure conditions.

---

## Key Insights
Several important patterns were identified during analysis:

- A small number of components account for a large proportion of failures and repair costs.
- Leak-related and sensor-related issues appear frequently.
- Steering and transmission issues are associated with critical component reliability.
- Noise and vibration patterns suggest potential mechanical wear or assembly problems.

---

## Recommendations
Based on the analysis, the following improvements could help reduce failures and costs:

- Strengthen assembly and quality inspection processes.
- Improve supplier quality control for frequently failing components.
- Add better protection for sensitive electronic components.
- Focus engineering efforts on components with high failure cost impact.
- Use generated tags to detect early warning signals of recurring issues.

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab / Jupyter Notebook

---

## Project Outcome
This project demonstrates an end-to-end data science workflow including:

- Data cleaning
- Exploratory data analysis
- Feature engineering from text
- Visualization
- Insight generation

The cleaned dataset and generated tags can support quality improvement, cost optimization, and reliability analysis.
