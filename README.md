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
**1. Given the provided data, what are three conclusions that we can draw about crowdfunding campaigns?**\
    1. Based on the dataset, I can conclude that the three most successful crowdfunding campaigns come from theater, music, and film & video categories; however, theater, music, and film & video are also the most failed and most canceled categories. Therefore, success is not guaranteed for new crowdfunding campaigns based solely on selecting a campaign within one of these three (parent) categories. 
    2. Based on the dataset, I can conclude that for each of the seven countries listed, the sub-category of ‘plays’ typically has the most successes and the most failures within the sub-categories, regardless of which country is being examined. This commonality is especially interesting when considering the varying sizes of these nations, varying languages, varying educational standards, varying political experiences, etc. 
    3. Based on the dataset, I can conclude that the most successful time of year for crowdfunding campaigns is in July. In addition, the relationship between the rate of failed campaigns and the rate of canceled campaigns seem to be the most correlated relationship. This suggests that similar factors may be affecting the likelihood of a campaign’s failure or cancellation. 

**2. What are some limitations of this dataset?**\
    1. There are various limitations that can affect the quality and the capabilities of a dataset; for example, this dataset may suffer from sampling bias, which suggests that the data may not be collected randomly or that the data is built with biased samples that may not truly represent the population. These complications may hinder the accuracy or the effectiveness of the dataset.
    2. In addition, any outliers may skew the results, therefore, sabotaging the analysis of the dataset. As a result, any insights or deductions pulled from the dataset may be misleading or inaccurate.
    3. Finally, this dataset may be prone to selection bias; for example, based on the names and descriptions in ‘blurbs’, there is a possibility that these values were carefully chosen based on the specific information they provide.
    4. Therefore, the dataset may be biased, thus narrowing and distorting any conclusions the dataset may generate.In conclusion, there are numerous limitations that may exist in a dataset; sampling bias, outliers, and/or selection bias may be some of the more likely limitations of this dataset, thus skewing any analysis.
 
 **3. What are some other possible tables and/or graphs that we could create, and what additional value would they provide?**\
    1. Another valuable way to analyze this dataset is to organize the highest ‘percent funded’ by country, and then use the ‘blurbs’ to understand which organizations or groups typically exceed their funding ‘goals’. This table/graph would make it easier to deduce which groups are most likely to exceed their funding goals, in each country. Thus, this analysis would suggest which type of groups/organizations, in each country, are most likely to succeed in their crowdfunding campaign. Who has the best chance?
  
**4. Use your data to determine whether the mean or the median better summarizes the data.**\
    1. In this case, the data is more accurately represented by the mean, because there is such a range between the data points. The median for both the successful and failed campaigns falls far below the actual average; therefore, the mean is more instructive with this data.

**5. Use your data to determine if there is more variability with successful or unsuccessful campaigns. Does this make sense? Why or why not?**\
    1. There is more variability with the successful campaigns than the unsuccessful; perhaps this does make sense, because it seems likely that a more successful campaign would have more backers. The juxtaposition of the variance and standard deviation of both campaigns illustrates this variability.

