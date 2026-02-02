## Data Analytics Process

To address the business challenge, I will follow a five stage analytics pipeline.

### 1. Data Collection

**Data Source:**
- **Dataset:** IBM HR Analytics Employee Attrition & Performance dataset (From Kaggle)
- **Structure:** Structured data (CSV format) containing 1,470 employee records across 35 features
- **Tooling:** Jupyter Notebook environment

**Key Features:**
- **Demographics:** Age, Gender, Marital Status, Education Level, Distance From Home
- **Compensation:** Monthly Income, Stock Option Level, Percent Salary Hike, Hourly/Daily Rate
- **Work Environment:** Overtime Status, Business Travel Frequency, Work-Life Balance Rating
- **Job Characteristics:** Job Role, Department, Job Level, Years at Company, Years in Current Role
- **Satisfaction Metrics:** Job Satisfaction, Environment Satisfaction, Relationship Satisfaction, Job Involvement
- **Performance:** Performance Rating, Training Times Last Year
- **Target Variable:** Attrition (Yes/No)

### 2. Data Preprocessing

**Data Quality Assessment:**
- Verify data completeness and check for missing values
- Examine data types

**Data Cleaning Steps:**

a. **Redundancy Removal:**
   - Remove zero variance features that do not contribute to variability analysis
   - Check for duplicate records

b. **Missing Value Treatment:**
   - Identify missing values across all columns
   - For numerical features: Impute with mean/median based on distribution
   - For categorical features: Impute with mode or create "Unknown" category

c. **Categorical Encoding:**
   - Create binary encoding for target variable: Attrition (Yes=1, No=0)
   - Retain original categorical variables (BusinessTravel, Department, JobRole, Gender, MaritalStatus) for grouping and segmentation analysis

