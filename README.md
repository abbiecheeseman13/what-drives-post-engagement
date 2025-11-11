# What Drives Post Engagement?

This project explores 500 Facebook posts from a cosmetic brand to uncover which factors most influence audience engagement. Using Python (Pandas, scikit-learn) for analysis and Tableau for visualization, it identifies what types of posts, timing, and strategies drive reach and interaction.

## Project Objective
To determine what post attributes (type, timing, paid vs. organic) most impact engagement rate, defined as:

The goal is to translate data patterns into actionable insights that could inform a content or marketing strategy.

## Dataset Overview
- Source: Facebook Metrics of a Cosmetic Brand (Kaggle)
- Records: 500 posts  
- Features: 20 columns including post type, weekday/hour of posting, paid status, reach, impressions, likes, comments, shares, and total interactions.
- Engineered Features: Engagement rate, categorized weekdays/hours, and paid vs. organic labels.

## Tools and Methods
| Tool | Purpose |
|------|----------|
| Python (Pandas, Matplotlib) | Cleaning, feature engineering, and exploratory data analysis |
| scikit-learn (Linear Regression, Random Forest) | Predictive modeling and feature importance |
| Tableau | Interactive visualization dashboard |
| Jupyter Notebook | Analytical workflow and documentation |

## Key Visual Insights

### 1. Engagement by Post Type
Photo posts generated the highest engagement rate (~2.6%), followed by status updates (~1.6%). Video and link posts underperformed.

Interpretation:  
For this cosmetic brand, highly visual photo content outperformed video, suggesting the audience prefers polished still imagery over motion content.

### 2. Optimal Posting Times
Peak engagement occurs between 3–10 AM across most weekdays.

Interpretation:  
Morning posts performed better—unusual compared to typical evening patterns—likely due to the brand’s global or early-bird audience base. Posts scheduled between 6–9 AM consistently ranked in the top engagement quartile.

### 3. Paid vs. Organic Reach
Paid posts achieved approximately twice the reach of organic posts but similar engagement rates (~2%).

Interpretation:  
Boosting content expands visibility but does not proportionally increase engagement rate. The quality and creative value of the post matter more than the promotion budget.

### 4. Reach vs. Engagement Relationship
High reach does not guarantee high engagement.

Interpretation:  
Scatter plots show that as reach increases, engagement rate tends to flatten or decline—indicating diminishing returns. This means not every viral post sustains strong per-user engagement.

### 5. Top 10 Posts by Interactions
The top-performing posts were all photo-based product highlights, averaging over 2,000 total interactions.

Interpretation:  
Visually strong and product-centric content drives both reach and user engagement. This insight can guide content replication for future campaigns.

## Modeling Insights
Two predictive models were tested to identify which features best predict engagement rate.

| Model | R² | Key Predictors |
|--------|----|----------------|
| Linear Regression | ~0.40 | Post Type, Post Hour, Paid Status |
| Random Forest Regressor | ~0.60 | Lifetime Reach, Post Type, Post Hour, Weekday |

Top Predictors (Feature Importance):
1. Lifetime Post Total Reach  
2. Post Type  
3. Post Hour  
4. Paid Status  
5. Weekday

These results confirm that content format and timing play larger roles than audience size alone.

## Business Recommendations
| Area | Recommendation | Rationale |
|------|----------------|-----------|
| Content | Prioritize photo-based content that aligns with product storytelling. | Photos have 2–3× higher engagement rates. |
| Timing | Schedule posts for early morning hours (6–9 AM). | Highest engagement during that window. |
| Paid Strategy | Use paid boosts to increase reach of top-performing posts. | Paid posts do not guarantee engagement—use strategically. |
| Monitoring | Maintain a Tableau dashboard to track engagement by type, hour, and post category. | Enables ongoing optimization. |

## Key Takeaways
- Photos outperform videos for this brand’s audience.  
- Morning posts yield stronger engagement than evening ones.  
- Reach and engagement are correlated but not linear.  
- Paid content expands visibility but does not inherently boost engagement.  
- Post timing and creative type are the strongest controllable factors.
