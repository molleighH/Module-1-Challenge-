# MSU Data Analysis Bootcamp 
## Module 1 Challenge: Microsoft Excel  
# Crowdfunding Analysis Project

This project involves analyzing a dataset of 1,000 crowdfunding projects to uncover trends, insights, and factors that influence the success or failure of campaigns. This analysis was conducted using Excel as part of a data analysis bootcamp, with the goal of identifying actionable insights that could help future campaigns succeed.

## Table of Contents

- [Project Overview](#project-overview)
- [Data Preparation](#data-preparation)
- [Analysis](#analysis)
  - [Conditional Formatting](#conditional-formatting)
  - [Column Creation](#column-creation)
  - [Pivot Tables and Charts](#pivot-tables-and-charts)
  - [Crowdfunding Goal Analysis](#crowdfunding-goal-analysis)
  - [Statistical Analysis of Backers](#statistical-analysis-of-backers)
- [Key Findings](#key-findings)
- [Limitations and Recommendations](#limitations-and-recommendations)
- [Analytic Report ](#analytic-report)

## Project Overview

Crowdfunding platforms like Kickstarter and Indiegogo have grown significantly in popularity since the late 2000s. However, not all projects succeed in reaching their funding goals. This project aims to analyze a sample of crowdfunding campaigns to identify trends that can predict success, failure, or cancellation. The analysis involves data cleaning, statistical analysis, and the creation of pivot tables and charts to visualize trends.

## Data Preparation

### Outcome Column Formatting
- Applied conditional formatting to the `Outcome` column to distinguish between successful, failed, canceled, and live campaigns.
- The color-coding enhances readability and highlights the distribution of outcomes across the dataset.

### Percent Funded Calculation
- Added a `Percent Funded` column to calculate the percentage of the funding goal achieved by each campaign.
- Applied a three-color scale (red to green to blue) to visualize funding levels, providing an immediate sense of which campaigns exceeded expectations.

### Average Donation Calculation
- Created an `Average Donation` column to determine the average contribution per backer.
- This metric helps gauge the engagement level of backers in successful versus unsuccessful campaigns.

### Category and Sub-Category Splitting
- Separated the `Category and Sub-Category` column into `Parent Category` and `Sub-Category` for more granular analysis.
- This allows for a deeper dive into the performance of specific categories and sub-categories.

### Date Conversion
- Converted Unix timestamps in the `launched_at` and `deadline` columns into readable date formats using Excel formulas.
- This step was crucial for time-based trend analysis.

## Analysis

### Conditional Formatting
- Applied to the `Outcome` and `Percent Funded` columns, making trends and outliers immediately visible.

### Column Creation
- New columns (`Percent Funded`, `Average Donation`, `Parent Category`, `Sub-Category`, `Date Created Conversion`, `Date Ended Conversion`) were created to facilitate deeper analysis and enhance data interpretability.

### Pivot Tables and Charts
- Created pivot tables and stacked-column charts to visualize the success rates of campaigns across different categories and sub-categories.
- Included filters for country and parent category, allowing for customized views of the data.

### Crowdfunding Goal Analysis
- Analyzed the relationship between funding goals and campaign outcomes.
- Created a line chart to depict how the amount of funding sought impacts the likelihood of success, failure, or cancellation.

### Statistical Analysis of Backers
- Generated summary statistics (mean, median, min, max, variance, standard deviation) for the number of backers in successful vs. unsuccessful campaigns.
- This analysis provided insights into the central tendencies and variability of backer engagement.

## Key Findings

1. **Success Trends**: Campaigns with lower funding goals (under $10,000) had a higher likelihood of success, while those with higher goals had increased chances of failure or cancellation.
2. **Category Performance**: Certain categories, such as Technology and Design, had higher success rates, especially when coupled with modest funding goals.
3. **Backer Engagement**: Successful campaigns generally had more consistent and higher backer engagement, as evidenced by lower variability in the number of backers.

## Limitations and Recommendations

### Limitations
- The dataset is a sample of 1,000 projects, which may not fully represent the entire crowdfunding landscape.
- Some campaigns were marked as live, preventing a final outcome analysis.

### Recommendations
- **Additional Analysis**: Incorporating external factors, such as social media presence and marketing efforts, could provide further insights into what drives campaign success.
- **Time-Series Analysis**: A deeper analysis of trends over time could reveal the impact of seasonal factors on campaign outcomes.
- **Sentiment Analysis**: Analyzing the tone and content of campaign descriptions and updates could predict backer engagement and success.

### Analytic Report 

**1. Given the provided data, what are three conclusions that we can draw about crowdfunding campaigns?**
   1. Based on the dataset, the three most successful crowdfunding campaigns come from the Theater, Music, and Film & Video categories. However, these categories are also the most failed and most canceled. Therefore, success is not guaranteed based solely on selecting a campaign within one of these three categories.
   2. For each of the seven countries listed, the sub-category of ‘Plays’ typically has the most successes and the most failures within the sub-categories, regardless of the country. This commonality is intriguing considering the varying sizes of these nations, languages, educational standards, political experiences, etc.
   3. The most successful time of year for crowdfunding campaigns is July. Additionally, there is a strong correlation between the rate of failed campaigns and the rate of canceled campaigns, suggesting that similar factors may be affecting the likelihood of a campaign's failure or cancellation.

**2. What are some limitations of this dataset?**
   1. The dataset may suffer from **sampling bias**, meaning that the data might not have been collected randomly or could be built with biased samples that do not truly represent the population, hindering accuracy.
   2. **Outliers** may skew the results, potentially leading to misleading or inaccurate analysis.
   3. The dataset could be prone to **selection bias**; for instance, the names and descriptions in ‘blurbs’ might have been carefully chosen based on specific information they provide, thus distorting any conclusions.
   4. In summary, sampling bias, outliers, and selection bias are some of the likely limitations of this dataset, potentially skewing any analysis.

**3. What are some other possible tables and/or graphs that we could create, and what additional value would they provide?**
   1. A valuable analysis could involve organizing the highest ‘percent funded’ by country and using the ‘blurbs’ to identify which organizations or groups typically exceed their funding goals. This table/graph would help determine which types of groups/organizations in each country are most likely to succeed in their crowdfunding campaigns.

**4. Use your data to determine whether the mean or the median better summarizes the data.**
   1. In this case, the **mean** better represents the data because of the wide range between data points. The median for both successful and failed campaigns falls far below the actual average, making the mean more instructive for this dataset.

**5. Use your data to determine if there is more variability with successful or unsuccessful campaigns. Does this make sense? Why or why not?**
   1. There is more variability with the successful campaigns than the unsuccessful ones. This makes sense because a more successful campaign is likely to have more backers, which is reflected in the higher variance and standard deviation of successful campaigns compared to unsuccessful ones.
