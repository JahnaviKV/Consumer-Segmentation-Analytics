##  Table of Contents

1. [ Executive Summary](#-executive-summary)
2. [ Objectives](#-objectives)
3. [ Methodology](#-methodology)
   - [Data Preparation](#data-preparation)
   - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
   - [Segmentation Analysis](#segmentation-analysis)
4. [ Predictive Modeling](#-predictive-modeling)
5. [ Business Impact](#-business-impact)
6. [ Recommendations](#-recommendations)
7. [ Key Insights](#-key-insights)
8. [ Tools & Technologies](#-tools--technologies)
9. [ Conclusion](#-conclusion)


##  Executive Summary

In today’s competitive market, understanding **consumer behavior** is key to optimizing marketing strategies and improving brand loyalty.  
This project, conducted for **AXANTEUS**, a market research agency, focuses on developing a **behavior-based segmentation model** to overcome the limitations of traditional demographic segmentation.

Using data on demographics, purchasing patterns, and promotional responses, the analysis identifies **value-conscious** and **brand-loyal** consumer groups, enabling clients to:

- Allocate marketing budgets effectively  
- Personalize promotional campaigns  
- Strengthen customer loyalty  

---

##  Objectives

###  Business Goals
- Transition from **demographic-based** to **behavior-based segmentation**
- Identify **value-conscious** and **brand-loyal** customers
- Develop **predictive models** for targeted marketing and promotion optimization  

###  Analytical Goals
- Segment consumers by **purchase behavior** and **basis for purchase** using clustering  
- Classify **value-conscious consumers** using supervised learning  
- Predict **brand loyalty** and **purchase volume** using regression models  

---

##  Methodology

### 1️ Data Preparation
- **Dataset:** 600 observations, 46 variables (demographic, purchase, and promotion data)  
- **Cleaning:** Managed missing values, removed zero entries, and renamed variables for clarity  
- **Transformation:** Standardized features for clustering; used **PCA** to assess dimensionality (no reduction required)

### 2️ Exploratory Data Analysis (EDA)
- Analyzed **distributions, correlations**, and **outliers**  
- Visualized key relationships between **demographics** and **purchasing behavior**

### 3️ Segmentation Analysis
Performed **K-Means Clustering** across three perspectives:

####  Purchase Behavior Segmentation
| Cluster | Description |
|----------|--------------|
| 1 | High-volume, cost-conscious shoppers |
| 2 | Average buyers with moderate brand engagement |
| 3 | Loyal, promotion-driven consumers |

####  Basis for Purchase Segmentation
| Cluster | Description |
|----------|--------------|
| 1 | Balanced mid-tier buyers |
| 2 | Premium consumers valuing exclusivity |
| 3 | Price-sensitive, promotion-focused buyers |

####  Combined Segmentation
| Cluster | Segment Type | Behavior Description |
|----------|---------------|----------------------|
| 1 | Balanced Consumers | Moderate engagement, balanced spending |
| 2 | Value-Oriented | Promotion-driven, cost-conscious |
| 3 | Premium Brand-Loyal | Exclusive, loyal, and high-value customers |

---

##  Predictive Modeling

###  Classification – Predicting Value-Conscious Consumers

| Model | Accuracy | AUC | Sensitivity | Specificity |
|--------|----------|-----|-------------|--------------|
| Logistic Regression | 58.9% | 0.63 | — | — |
| Decision Tree | 63.9% | 0.61 | — | — |
| **Random Forest** | **65.6%** | **0.65** | **76.4%** | **50.0%** |

>  **Best Model:** Random Forest — most effective at identifying **value-conscious** consumers.

---

###  Regression – Predicting Total Purchase Volume

| Model | R² | Notes |
|--------|----|-------|
| Linear Regression | **0.844** | Best overall fit with low RMSE and MAE |
| Regression Tree | — | Revealed interpretable rules identifying key drivers (Total Purchase Value, Education Level, Socioeconomic Class) |

---

##  Business Impact

The behavior-based segmentation model enables AXANTEUS to:

- Understand consumers **beyond demographics**
- Target **cost-sensitive clusters** (value-conscious)
- Reward **brand-loyal consumers**
- Optimize **marketing spend** through precise targeting

| Cluster | Segment Type | Marketing Focus |
|----------|---------------|----------------|
| 1 | General Buyers | Mid-range offers, bundle promotions |
| 2 | Value-Oriented | Discounts, loyalty programs |
| 3 | Brand-Loyal Buyers | Premium access, exclusive rewards |

---

##  Recommendations

- **Value-Conscious Consumers:** Emphasize discounts, flash sales, and loyalty rewards.  
- **Brand-Loyal Consumers:** Highlight product quality, exclusivity, and VIP experiences.  
- **General Buyers:** Maintain engagement with regular, balanced promotions.  
- Continuously **update segmentation models** as consumer behavior evolves.

---

##  Key Insights

- Behavior-based segmentation reveals deeper insights into **purchase motivations**.  
- Predictive models enable **targeted campaign design** and **customer retention strategies**.  
- The **Random Forest model** offers the most reliable classification of value-conscious consumers.  
- Data-driven segmentation enhances **AXANTEUS’s strategic marketing decisions**.

---

##  Tools & Technologies

**Language:** R  

**Libraries:**  
`dplyr`, `ggplot2`, `factoextra`, `cluster`, `caret`, `randomForest`

**Techniques Used:**  
- Exploratory Data Analysis (EDA)  
- K-Means Clustering  
- Principal Component Analysis (PCA)  
- Logistic Regression, Decision Trees, Random Forest  
- Linear & Regression Tree Modeling  

---

##  Conclusion

This project successfully developed a **comprehensive consumer segment**
