🍜 Data Storytelling with Ramen | Product Ratings Analysis  
I explored a global dataset of instant ramen products and went beyond visuals — using real statistics to uncover what truly influences ratings. Here's what I found:

### 🔍 Key Insights:
- 84% of ramen products were rated Excellent or Good.  
- 🇯🇵 Japan leads with the most highly rated products, followed by 🇰🇷 South Korea and 🇺🇸 the USA.  
- Brand Nissin stood out with over 200 top-rated products.  
- Pack-style ramen received the highest average ratings — higher than Cup or Bowl.

### 📊 What makes this more than just charts?
I used statistical modeling to validate the patterns I observed.

Instead of using a simple linear regression, I applied an **Ordinal Logistic Regression** — a model specifically designed for ranked data like star ratings.  
It helped quantify the true effect of **Country, Brand, and Packaging Style** on ramen ratings.

✅ The model was highly significant (**p < 0.001**), showing that these features **meaningfully influence** how ramen is rated by consumers.

For example:
- Ramen from the USA had significantly lower ratings.
- Brands like **Nissin** and **Nongshim** were strongly associated with higher satisfaction.
- Cup-style ramen received statistically lower ratings than Pack-style.

I also ran an independent t-test comparing Pack vs Bowl packaging styles.  
Interestingly, while Pack had a slightly higher average, the difference was **not statistically significant**.

> _"Visualization shows the pattern — but statistics prove it."_

### 📁 Want to see the full notebook?  

