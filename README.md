# Coursera Dataset Exploration

## Overview
This project explores a dataset of Coursera learning programs to uncover trends, insights, and actionable takeaways about program popularity, student enrollment, and certificate types. The analysis aims to answer the key business question:

**Which type of learning program is most likely to attract and retain students?**

The dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/siddharthm1698/coursera-course-dataset) and includes 6 columns describing 890 Coursera programs.

---

## Business Question
- What learning program onboarded would be most successful?

---

## Key Insights & Takeaways
1. **Professional Certificates attract the most students on average**  
   Despite being less common, they consistently show higher enrollment numbers than courses or specializations.

2. **Professional Certificates are underrepresented**  
   They have the lowest prevalence, suggesting a potential growth opportunity.

3. **Courses dominate in availability, especially for beginners and mixed-level learners**  
   Courses cater broadly to beginners and mixed-level students, accounting for the largest share of total enrollments.

---

## Dataset
- **Raw Source:** Scraped from Coursera website
- **Columns:** `Program`, `Organization`, `Type`, `Rating`, `Difficulty`, `Students`
- **Observations:** 890 learning programs
- **Cleaned Data:** A preprocessed version of the dataset is available at `data/coursera_data_cleaned.csv` for direct use in analysis.

---

## Cleaning & Preparation
- Renamed columns for readability.
- Converted `Students` column from string to integer, handling suffixes (`k`, `M`).
- Corrected `Type` column capitalization.
- Checked for duplicates, null values, and outliers.
- Converted appropriate columns to categorical or numeric types for better performance.
- Exported cleaned CSV for reproducibility.

---

## Analysis
- Explored **ratings** across program types and difficulties.
- Examined **student enrollment** distribution, including medians and outliers.
- Conducted **correlation analysis** between ratings and enrollment numbers.
- Investigated **organization contributions** and program counts.
- Aggregated enrollments by **program type** and **difficulty**.

Visualizations include:
- Boxplots for ratings and enrollments
- Scatterplots for rating vs. enrollment
- Stacked bar charts for total enrollments by program type and difficulty

---

## Limitations
- No timestamp data, preventing temporal analysis.
- No unique student IDs; some students may appear in multiple programs.
- No competitor or industry-specific data.
- Limited to Coursera platform only.

---

## Next Steps
- Re-evaluate trends after 6 months.
- Scrape competitor data for comparison.
- Expand analysis to industry categorization and program completion rates.

---

## Getting Started
1. Clone the repository
2. Install dependencies:
```bash
pip install pandas numpy seaborn matplotlib
```
3. Run the notebook `Coursera_Dataset_Exploration.ipynb` in Jupyter or VS Code.
4. Optionally, use the cleaned dataset directly (`data/coursera_data_cleaned.csv`) to skip the cleaning steps.

