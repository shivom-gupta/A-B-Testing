# A/B Testing Analysis: E-Commerce Website

### Overview

This project involves analyzing the results of an A/B test conducted by an e-commerce website. The primary objective is to evaluate whether a newly designed webpage results in a higher conversion rate compared to the existing page. The company aims to determine whether to implement the new webpage, retain the old one, or continue the experiment to gather more data before making a decision.

### Dataset Description

The dataset used in this analysis includes the following columns:

- **user_id**: Unique identifier for each user.
- **timestamp**: The time when the user visited the webpage.
- **group**: Indicates whether the user was part of the control group (old_page) or the treatment group (new_page).
- **landing_page**: Specifies whether the user was shown the old or new webpage.
- **converted**: Indicates whether the user converted (1 for yes, 0 for no).

### Project Workflow

1. **Data Loading and Exploration:**
   - Load the dataset and conduct an initial exploration to understand its structure.
   - Inspect the dataset for any inconsistencies or inaccuracies, such as mismatches between the `group` and `landing_page` columns.

2. **Data Cleaning:**
   - Identify and remove any rows where the `group` and `landing_page` do not align (e.g., `treatment` group users shown the `old_page`).
   - Verify that there are no duplicates and check for any missing values.

3. **Exploratory Data Analysis (EDA):**
   - Calculate basic statistics, such as the proportion of users who converted overall, and within each group.
   - Investigate any potential discrepancies in the data, such as the number of times a `treatment` group user was not served the `new_page`.

4. **Hypothesis Testing:**
   - Formulate null and alternative hypotheses:
     - **Null Hypothesis (H0)**: The new webpage does not result in a higher conversion rate than the old webpage.
     - **Alternative Hypothesis (H1)**: The new webpage results in a higher conversion rate than the old webpage.
   - Conduct a z-test to determine if the difference in conversion rates between the control and treatment groups is statistically significant.

5. **Results Interpretation:**
   - Analyze the p-value and confidence intervals to determine whether to reject the null hypothesis.
   - Consider both statistical and practical significance in the decision-making process.

6. **Conclusion and Recommendations:**
   - Based on the analysis, provide recommendations on whether the company should:
     - Implement the new webpage,
     - Retain the old webpage, or
     - Continue running the experiment to gather more data.

### Conclusion

The notebook provides a comprehensive analysis of the A/B test results, guiding the company towards an informed decision regarding the implementation of the new webpage. This analysis not only assesses statistical significance but also considers the practical implications of the findings.
