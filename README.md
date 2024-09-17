# Mall Customers Analysis

## Project Overview
This project analyzes customer data from a mall to gain insights into customer behavior, segmentation, and spending patterns. The analysis aims to help the mall's management make data-driven decisions for marketing strategies and customer engagement.

## Dataset
The dataset contains information about mall customers, including:
- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1-100)

## Methodology
1. Data Preprocessing: Cleaned and prepared the dataset for analysis.
2. Exploratory Data Analysis (EDA): Conducted various visualizations to understand the relationships between different variables.
3. Customer Segmentation: Applied K-means clustering to segment customers based on their annual income and spending score.

## Key Findings

### 1. Customer Segmentation
- Identified 5 distinct customer segments based on annual income and spending score.
- Segments include: low income/low spending, low income/high spending, medium income/medium spending, high income/low spending, and high income/high spending.

### 2. Annual Income vs. Spending Score
- No strong correlation between annual income and spending score.
- Gender doesn't seem to significantly influence the relationship between income and spending.

### 3. Age vs. Annual Income
- Wide range of incomes across all age groups.
- Some higher incomes observed in the 30-50 age range, but not exclusively.

### 4. Age vs. Spending Score
- Younger customers (20-40) tend to have a wider range of spending scores.
- Older customers (50+) show a slight trend towards lower spending scores.

### 5. Optimal Number of Clusters
- The elbow method graph suggests that 5 clusters is optimal for this dataset, as the rate of WCSS decrease levels off after this point.

### 6. Comprehensive Variable Relationships (Pairplot)
- Age Distribution: The majority of customers are between 30 and 50 years old, with a slight skew towards younger customers.
- Income Distribution: Annual incomes are relatively evenly distributed, with a peak around 70k$.
- Spending Score Distribution: There's a bimodal distribution in spending scores, with peaks around 25-30 and 70-75.
- Age vs. Income: There's a slight positive correlation between age and income, but with high variability.
- Age vs. Spending Score: Younger customers tend to have higher spending scores, with a gradual decrease as age increases.
- Income vs. Spending Score: There's no clear linear relationship between income and spending score.
- Gender Differences: 
  - Age: The age distribution is similar for both genders.
  - Income: Males show a slightly higher average income, but with considerable overlap.
  - Spending Score: Females tend to have slightly higher spending scores on average.

### 7. Customer Segment Profiles
Based on the K-means clustering, we've identified five distinct customer segments:

| Cluster | Age (Avg) | Annual Income (k$) | Spending Score | Dominant Gender | Count |
|---------|-----------|---------------------|----------------|-----------------|-------|
| 0       | 41.11     | 88.20               | 17.11          | Male            | 35    |
| 1       | 42.72     | 55.30               | 49.52          | Female          | 81    |
| 2       | 32.69     | 86.54               | 82.13          | Female          | 39    |
| 3       | 25.27     | 25.73               | 79.36          | Female          | 22    |
| 4       | 45.22     | 26.30               | 20.91          | Female          | 23    |

Segment Characteristics:
- Cluster 0: High-Income, Low-Spending, Middle-Aged Males
- Cluster 1: Average-Income, Average-Spending, Middle-Aged Females (Largest Group)
- Cluster 2: High-Income, High-Spending, Young Adult Females
- Cluster 3: Low-Income, High-Spending, Young Adult Females
- Cluster 4: Low-Income, Low-Spending, Middle-Aged Females

## Insights and Recommendations

1. Targeted Segment Strategies:
   - Cluster 0 (High-Income, Low-Spending Males): Focus on increasing engagement and spending. Implement luxury product promotions and exclusive experiences to encourage higher spending.
   - Cluster 1 (Average Segment): As the largest group, prioritize retention strategies. Offer a mix of value-based and aspirational products to cater to their average spending habits.
   - Cluster 2 (High-Value Segment): Prioritize retention and premium experiences. Implement VIP programs and early access to new products/services.
   - Cluster 3 (Young, High-Spending): Focus on building brand loyalty. Offer trendy, fashionable products and leverage social media marketing.
   - Cluster 4 (Budget Segment): Emphasize value for money. Implement budget-friendly promotions and loyalty programs to increase visit frequency.

2. Gender-Focused Approach: Given that four out of five clusters are dominated by females, ensure the mall's overall marketing and product mix caters strongly to female preferences, while still maintaining offerings for the male demographic.

3. Age-Based Marketing: Tailor marketing strategies to the average age of each cluster. For example, use more traditional marketing channels for Clusters 0, 1, and 4, while leveraging digital and social media marketing for Clusters 2 and 3.

4. Income-Appropriate Offerings: Ensure a good mix of high-end and budget-friendly stores/products to cater to the diverse income levels across segments.

5. Spending Score Improvement: For Clusters 0 and 4 with low spending scores, implement targeted campaigns to increase their engagement and spending in the mall.

6. Targeted Age-Based Marketing: Given the relationship between age and spending score, develop age-specific marketing campaigns. Focus on maintaining high spending among younger customers while creating strategies to increase spending among older demographics.

7. Income-Independent Strategies: Since there's no strong correlation between income and spending score, focus on factors beyond income (e.g., customer experience, product appeal) to increase spending across all income levels.

8. Gender-Specific Approaches: While differences are not dramatic, slightly tailor approaches for male and female customers:
   - For male customers: Focus on increasing spending scores, possibly through targeted promotions or loyalty programs.
   - For female customers: Capitalize on their higher spending tendency with exclusive or limited-time offers.

9. Bimodal Spending Strategy: Address the two peaks in the spending score distribution:
   - For low spenders (around 25-30 score): Implement strategies to encourage increased spending, such as value-based promotions or bundled offerings.
   - For high spenders (around 70-75 score): Focus on retention and luxury or premium offerings to maintain their high spending levels.

## Future Work
1. Incorporate more customer data, such as visit frequency and preferred store categories.
2. Conduct time-series analysis to understand seasonal trends in customer behavior.
3. Implement predictive models to forecast customer spending and churn.
4. Conduct deeper analysis into the factors influencing the spending patterns of each cluster.
5. Develop personalized marketing campaigns for each customer segment based on their unique characteristics.
6. Investigate the reasons behind the gender imbalance in most clusters and develop strategies to attract more male customers if desired.

## Tools Used
- Python
- Pandas for data manipulation
- Matplotlib and Seaborn for data visualization
- Scikit-learn for K-means clustering

This analysis provides valuable insights into customer behavior at the mall, enabling data-driven decision-making for marketing, customer engagement, and overall business strategy.
