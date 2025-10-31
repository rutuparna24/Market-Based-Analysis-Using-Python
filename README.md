# Market-Based-Analysis-Using-Python

📘 Overview

This project implements Market Basket Analysis (MBA) using Python to uncover purchasing patterns and product associations in transactional data. By analyzing customer transactions, it identifies items frequently bought together—offering data-driven insights to optimize product recommendations, cross-selling strategies, and marketing campaigns.
The analysis leverages the Apriori algorithm to generate frequent itemsets and association rules, supported by detailed visualizations for better interpretation.

📊 Dataset Description

The dataset consists of retail transactions, where each record represents the items purchased and their quantities within a single transaction. This data serves as the foundation for identifying frequent itemsets and association rules that reveal co-purchasing behavior.

Column Name	Description
Transaction ID	Unique identifier for each transaction
Item	Product purchased
Quantity	Number of units bought

Sample data:

Transaction ID	Item	Quantity
1	Bread	1
1	Butter	2
2	Milk	1
2	Eggs	1
3	Coffee	1
3	Sugar	1
🔍 Analysis Workflow
1. Data Preprocessing

Cleaned and structured raw data using Pandas.

Handled missing values and converted transactions into item-level records.

2. Exploratory Data Analysis (EDA)

Analyzed item frequencies and transaction distributions.

Visualized top-selling products using bar charts and histograms to understand purchasing trends.

3. Apriori Algorithm

Applied the Apriori algorithm to detect frequent itemsets.

Generated association rules based on support, confidence, and lift to evaluate item relationships.

4. Visualization

Presented findings through bar plots, heatmaps, and scatter plots for intuitive understanding of correlations.

🧠 Key Concepts

Support: Fraction of transactions containing a given itemset.

Confidence: Probability that a product is purchased given another is in the basket.

Lift: Degree to which two items are bought together compared with random chance.

📈 Frequent Itemsets (Support ≥ 0.05)
Itemset	Support
Bread, Butter	0.08
Milk, Eggs	0.12
Coffee, Sugar	0.10
Tea, Biscuits	0.07
Bread, Milk	0.09
🔗 Association Rules (Confidence ≥ 0.7, Lift > 1)
Rule	Confidence	Lift
{Bread} → {Butter}	0.70	1.30
{Milk} → {Eggs}	0.85	1.45
{Coffee} → {Sugar}	0.60	1.20
{Tea} → {Biscuits}	0.75	1.35
{Bread, Butter} → {Milk}	0.65	1.28
📊 Visualization Highlights

Top 10 Most Frequent Items:
Bar chart illustrating the most commonly purchased products.

Item Association Heatmap:
Displays correlation strength between products based on lift values.

Confidence vs Lift Scatter Plot:
Plots association rules to assess the reliability and impact of item pairings.

🧩 Results

{Milk → Eggs} shows the strongest association (Confidence = 85%, Lift = 1.45).

{Bread → Butter} indicates a consistent pattern (Confidence = 70%).

The heatmap highlights high-correlation product pairs, suggesting strategic opportunities for cross-promotion.

✅ Conclusion

Market Basket Analysis provides actionable insights into customer purchasing behavior. By identifying frequent itemsets and association rules, retailers can:

Improve product placement by grouping complementary items.

Develop personalized recommendations and targeted promotions.

Enhance cross-selling opportunities and inventory efficiency.

Understanding these associations enables data-driven decisions that boost sales and elevate the overall shopping experience.
