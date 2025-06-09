# 🍜 Ramen Ratings Analysis

##  Overview  
This project explores a dataset of global **instant ramen reviews** to uncover patterns in product quality across countries, brands, and packaging styles.  
The goal is to extract meaningful insights from consumer ratings using Python, visualization, and statistical modeling.

---

##  Objectives  
- Identify which **countries** produce the most top-rated ramen.  
- Analyze **brands** with consistent high-quality products.  
- Evaluate how **packaging styles** (e.g., Pack, Bowl, Cup) affect ratings.  
- Apply **statistical analysis** to test significance of differences.  
- Visualize **categorical distributions and trends** clearly and interactively.

---

##  Tools & Technologies  
- Python: `Pandas`, `NumPy`, `Seaborn`, `Matplotlib`, `Statsmodels`, `SciPy`  
- Jupyter Notebook  
- Data Cleaning & Transformation  
- Categorical Analysis & Statistical Testing  
- Barplots, Boxplots, GroupBy Visualizations  
- Hypothesis Testing & Regression Modeling  

---

##  Key Insights  
- Over **84%** of ramen products received either **Excellent** or **Good** ratings.  
- 🇯🇵 **Japan** leads in excellent-rated products, followed by **South Korea** 🇰🇷 and the **USA** 🇺🇸.  
-  **Nissin** is the top-performing brand with over **200** highly-rated entries.  
-  **Pack-style ramen** received the highest average star rating among all packaging types.

---

##  Statistical Analysis

### 🔬 Linear Regression (OLS)
We used an OLS regression model to test how **Country**, **Brand**, and **Style** affect ratings:

```python
import statsmodels.formula.api as smf
model = smf.ols('Stars ~ C(Country) + C(Style) + C(Brand)', data=df_clean).fit()
print(model.summary())

| Metric               | Value       | Interpretation                                                           |
| -------------------- | ----------- | ------------------------------------------------------------------------ |
| **R-squared**        | 0.442       | 44.2% of the variation in ratings is explained by the model              |
| **Adjusted R²**      | 0.344       | Adjusted for number of dummy variables (387 total)                       |
| **F-statistic**      | 4.495       | Model is overall statistically significant                               |
| **P-value (F-stat)** | 2.00e-112 ✅ | Strong evidence that at least one variable significantly affects ratings |

Conclusion: The model confirms that country of origin, brand, and style significantly influence ramen ratings.

 Author
Waseem Almazrua
Data Analyst | Healthcare Quality | AI Enthusiast
