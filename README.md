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

## Key Takeaways
- Content type and topic matter far more than timing. Photo posts and certain content categories dramatically outperform others and are the strongest predictors of engagement rate.
- Organic posts generate higher engagement rates than paid posts. Paid distribution increases reach but dilutes engagement quality by pushing content to colder audiences.
- Engagement rate is driven by deeper interactions, especially likes, comments, shares, engaged users, and consumers — confirming that ER reflects content quality, not raw reach.
- Audience loyalty plays a major role. Posts seen by people who already like the page produce significantly higher engagement, and reach from loyal followers is one of the strongest predictors.
- Timing (hour/weekday) has only minor influence. While late-night and morning posts perform slightly better, posting hour and weekday have weak correlations overall compared to content-related features.

## Business Recommendations
- Prioritize high-performing content types, especially photo-based posts, and expand content themes within categories that historically generate strong engagement.
- Double down on content crafted for your existing audience, focusing on relevance, storytelling, and visual style that resonates with followers to maximize engagement rate.
- Use paid promotion strategically, not to raise engagement rate but to expand reach when you have content that is already performing well organically.
- Optimize content quality signals, such as strong visuals, engaging copy, and hooks that encourage likes, comments, and shares — these behaviors heavily predict ER.
- Test different content categories and iterate, using your Random Forest results to identify which themes/topics (“Category_1”) are driving engagement and where to scale or pivot.
