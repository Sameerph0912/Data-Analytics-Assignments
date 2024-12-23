Here’s a `README.md` template for your project. This file will explain the project overview, data cleaning process, and key insights. You can modify it according to your project's details.

---

# Data Analyst Intern Assignment

## Project Overview

This project involves cleaning and analyzing user data for a fictional cooking application. The dataset consists of three main parts:

- **UserDetails**: Information about users (e.g., age, location, and preferences).
- **CookingSessions**: Details of dishes users have cooked and how they rate the sessions.
- **OrderDetails**: Information about what users have ordered, how often, and their preferences.

The goal of this project is to clean the raw data, perform some exploratory analysis, and save the cleaned datasets in a structured format. The final cleaned data is stored in an Excel file with separate sheets for each dataset.

---

## Tools Used

- **Python**: Programming language used for data cleaning and analysis.
- **pandas**: Library used for data manipulation and cleaning.
- **openpyxl**: Library for writing Excel files.

You can install the necessary libraries using:

```bash
pip install pandas matplotlib seaborn openpyxl
```

---

## Data Cleaning Process

### Step 1: Data Loading and Exploration
The data from multiple sheets in an Excel file was loaded using `pandas`. Missing values and data inconsistencies were identified by inspecting the data.

### Step 2: Handling Missing Values
- For the `OrderDetails` dataset, missing `Rating` values were filled with `0` as a default value.
- In the `UserDetails` dataset, missing values were filled with 'Unknown' to avoid errors during analysis.

### Step 3: Data Standardization
- The `User ID` and `Session ID` were standardized to ensure consistency across different datasets before merging them.

### Step 4: Merging Datasets
The three datasets (`UserDetails`, `CookingSessions`, and `OrderDetails`) were merged based on common keys (`User ID` and `Session ID`) to form a comprehensive dataset for analysis.

### Step 5: Saving Cleaned Data
The cleaned datasets were saved into separate sheets in an Excel file using the `ExcelWriter` functionality in `pandas`.

---

## Data Structure

The final cleaned data is saved in an Excel file (`cleaned_data.xlsx`) with the following sheets:

1. **UserDetails**: Contains information about users (e.g., age, location, preferences).
2. **CookingSessions**: Contains details about the dishes cooked by users and their ratings.
3. **OrderDetails**: Contains information about users' orders, such as item types and order frequency.

---

## Key Insights

- **Most Popular Dishes**: Identified which dishes are most frequently cooked by users.
- **Demographic Analysis**: Analyzed how location and age groups influence the amount spent on orders and their preferences.
- **Cooking Sessions vs Orders**: Investigated if users who engage in more cooking sessions tend to order more frequently.

---

## Visualizations

The following visualizations were created to provide insights from the data:

1. **Bar Chart**: Shows the most popular dishes cooked by users.
2. **Line Chart**: Displays the trend of orders over time.
---

## Conclusion and Recommendations

- **Dish Recommendations**: Based on the analysis, recommend promoting the most popular dishes in specific regions.
- **Targeted Marketing**: Use demographic analysis to tailor marketing strategies and meal offerings to different age groups and locations.

---

## Files Included

- **cleaned_data.xlsx**: The cleaned data stored in separate sheets.
- **README.md**: Project overview, cleaning process, and insights.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
