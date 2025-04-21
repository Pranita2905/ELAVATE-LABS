#  Customer Personality Analysis – Data Cleaning & Preprocessing

## Project Overview
This project focuses on cleaning and preprocessing the **Customer Personality Analysis** dataset from Kaggle to prepare it for further analysis or modeling.

The raw dataset contains customer demographic and behavioral data, including purchase history and campaign response metrics. Before analysis, we needed to clean the dataset to handle missing values, ensure consistent formatting, and standardize data types.


## Tools Used
- Python
- Pandas
- Jupyter Notebook

## Dataset Source
Kaggle: [Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)


## Cleaning Steps Performed

Step and Description
1. **Load & Parse**:- Fixed delimiter issue by using `sep='\t'` to properly read the tab-separated values.
2. **Missing Values**:- Filled missing values in the `Income` column using the median value. |
3. **Remove Duplicates**:- Removed any duplicate rows using `drop_duplicates()`. |
4. **Standardize Text**:- Lowercased and stripped whitespace from text columns like `Education` and `Marital_Status`. |
5. **Group Similar Categories**:- Combined similar marital status groups (e.g., 'Together' and 'Married', 'Widow' and 'Alone' → 'Other'). |
6. **Convert Date Format**:- Converted `Dt_Customer` to `datetime` using format `%d-%m-%Y`. |
7. **Rename Columns**:- Cleaned column names to be lowercase and snake_case (e.g., `Year_Birth` → `year_birth`). |
8. **Check Data Types**:- Ensured all numerical and categorical columns had appropriate types (e.g., `income` as float, `response` as int). |


## Output
-  `cleaned_marketing_campaign.csv` – Fully cleaned dataset.
---

## Next Steps
You can now:
- Perform **exploratory data analysis (EDA)**
- Build **customer segments**
- Train models for **campaign targeting**

---

## Contact
For questions or collaboration:  
**Pranita Vilas Mothe** – [mothepranita@gmail.com]
