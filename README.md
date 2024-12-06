# Corporate Survival Analysis

### Overview
This project uses survival analysis to predict the **bankruptcy risk** and **survival duration** of American companies. Leveraging a Kaggle dataset with financial attributes of companies listed on NYSE and NASDAQ from 1999 to 2018, we applied advanced statistical and machine learning methods to assess corporate longevity.

---

### Dataset
- **Source**: [American Companies Bankruptcy Prediction Dataset](https://www.kaggle.com/datasets/utkarshx27/american-companies-bankruptcy-prediction-dataset)  
- **Size**: 78,682 firm-year records across 8,262 unique companies  
- **Key Attributes**:
  - Financial variables like EBIT, Net Income, Gross Profit
  - Status labels: `0` (alive) or `1` (bankrupt)

---

### Project Objectives
1. Predict the **probability and timing of bankruptcy** for companies.
2. Understand the factors affecting corporate survival through survival analysis techniques.

---

### Methods
- **Kaplan-Meier Curve**: Visualizing survival probabilities over time.
- **Accelerated Failure Time (AFT)**: Predicting survival duration under distributional assumptions.
- **Cox Proportional Hazards Model**: Estimating hazard rates with penalties (LASSO).
- **Random Survival Forest (RSF)**: Modeling non-linear relationships and variable interactions.

---

### Key Results
- **Best Performing Model**: Random Survival Forest
  - C-index: 0.782 (highest accuracy)
  - Captures complex variable interactions.
- **Kaplan-Meier Curve**: Revealed a steady decline in corporate survival over time with >75% surviving beyond 20 years.

---

### How to Use
1. **Preprocessing**: Data cleaning, transformation (log and Yeo-Johnson), and ratio calculation.
2. **Survival Analysis**: Fit models and predict survival times or hazard rates.
3. **Evaluation**: Use the C-index metric to assess model performance.

---

### Tools & Technologies
- **Language**: R
- **Key Packages**:
  - `dplyr`, `survival`, `MASS`, `randomForestSRC`
- **Visualization**: Kaplan-Meier curves, correlation plots

---

### Conclusion
Survival analysis provides a robust framework for understanding bankruptcy risks. The **Random Survival Forest model** demonstrated the best predictive performance, highlighting the value of machine learning in corporate risk assessment.

---

