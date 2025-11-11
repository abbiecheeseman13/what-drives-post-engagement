# 🧠 What Drives Post Engagement?  
**Meta Data Scientist Project – Behavioral Insights from Facebook Metrics**

This project analyzes **500 Facebook posts** from a **cosmetic brand** to uncover what drives user engagement — likes, comments, shares, and total interactions.  
Using Python for analysis and Tableau for visualization, the project identifies the strongest predictors of post engagement and provides actionable recommendations for social media optimization.

---

## 📊 Project Overview
- **Goal:** Determine which post attributes (type, time, paid vs. organic) most influence engagement.  
- **Dataset:** [Facebook Metrics of a Cosmetic Brand]([https://www.kaggle.com/datasets](https://www.kaggle.com/datasets/dileeppatchaone/facebook-metrics-dataset-of-cosmetic-brand)) — 500 posts, 20 variables.  
- **Tools:**  
  - **Python:** Pandas, Matplotlib, scikit-learn  
  - **Modeling:** Linear Regression, Random Forest Regressor  
  - **Visualization:** Tableau Public Dashboard  
  - **Documentation:** ReportLab, Markdown

---

## 🧩 Data Summary
| Feature Group | Example Columns | Description |
|----------------|-----------------|--------------|
| Post Metadata | `Type`, `Category`, `Post Month`, `Post Hour`, `Post Weekday` | Structure and timing of posts |
| Reach Metrics | `Lifetime Post Total Reach`, `Lifetime Impressions`, `Engaged Users` | Visibility and audience scale |
| Engagement Metrics | `Like`, `Comment`, `Share`, `Total Interactions` | User engagement behavior |
| Target Variable | `Engagement Rate` | Defined as `Total Interactions / Lifetime Reach` |

---

## 🔍 Analysis Process
1. **Data Cleaning & Preparation**
   - Removed redundant columns (`Unnamed: 0`)
   - Filled or dropped minimal missing values
   - Engineered *Engagement Rate* as the primary target variable  
   - Encoded categorical features and normalized numeric ones  

2. **Exploratory Data Analysis (EDA)**
   - Engagement by **post type**, **hour**, and **weekday**
   - Correlation analysis of reach and interactions  
   - Paid vs. organic performance comparison  

3. **Modeling**
   - Built **Linear Regression** and **Random Forest** models to quantify feature importance.  
   - Random Forest achieved **R² ≈ 0.6**, outperforming Linear Regression (R² ≈ 0.4).  

4. **Dashboard Visualization**
   - Tableau dashboard summarizes findings interactively (post type, timing, paid vs. organic).

---

## 🌟 Key Findings
- **Post Type:** Video posts have the **highest engagement rates**, outperforming photos and links.  
- **Timing:** Engagement peaks between **6–9 PM on weekdays**, especially **Thursday/Friday**.  
- **Paid vs. Organic:** Paid boosts increase **reach** but not always **engagement rate**.  
- **Feature Importance:** Top predictors — *Post Type (Video)*, *Total Reach*, *Post Hour*, *Paid Status*.  

---

## 💡 Recommendations
| Focus Area | Recommendation | Impact |
|-------------|----------------|--------|
| Content Strategy | Increase proportion of **short-form video posts** | +20–30% engagement lift |
| Timing | Post during **evening hours mid–late week** | Align with peak activity |
| Paid Media | Boost **already successful posts** only | Improve ROI on ad spend |
| Monitoring | Automate weekly Tableau dashboard | Ongoing data-driven strategy |

---

## 📈 Tableau Dashboard
**Dashboard Title:** *“What Drives Post Engagement?”*  
Interactive visualization available on Tableau Public *(coming soon)*  

**Suggested Visuals:**
- Engagement by Post Type (Bar/Box Plot)  
- Engagement by Hour & Weekday (Heatmap)  
- Paid vs. Organic Comparison (Side-by-Side Bars)  
- Engagement vs. Reach (Scatter Plot)  
- Top 10 Posts by Total Interactions (Bar/Table)  
- Feature Importance from Random Forest (Bar Chart)

---

## 🧮 Model Results Summary
| Model | R² Score | MAE | Top Predictors |
|--------|-----------|-----|----------------|
| Linear Regression | ~0.40 | 0.006 | Post Type, Hour, Paid |
| Random Forest | ~0.60 | 0.004 | Reach, Post Type, Hour, Paid |
