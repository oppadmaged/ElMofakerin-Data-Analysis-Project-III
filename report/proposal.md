# 1. Project Title
A Comparative Statistical Analysis of Residential Property Pricing: New Cairo vs. Sheikh Zayed City

# 2. Background & Context
This project draws on about 20,000 real estate listings scraped from PropertyFinder Egypt. The dataset is packed with detailed info: asking price, GPS coordinates, property type, and size. By digging into these two urban centers, we can spot investment trends and see how property values stack up across Greater Cairo.

# 3. Research Question
Is there a real, measurable difference in average property prices between New Cairo City and Sheikh Zayed City?

# 4. Variables

**Variable Category:** Independent  
**Variable Name:** location  
**Data Type:** Categorical  
**Description:** The city where the property sits.

**Variable Category:** Dependent  
**Variable Name:** price  
**Data Type:** Continuous  
**Description:** The listing price in EGP.

# 5. Hypotheses
We’re testing at a 0.05 significance level.

**Null Hypothesis (H₀):** The average price in New Cairo is the same as in Sheikh Zayed.  
**Alternative Hypothesis (H₁):** The average prices are not the same.

# 6. Statistical Method
We’ll use an independent two-sample t-test to compare mean property prices between the two cities.

# 7. Statistical Assumptions
- The price data in each city should be normal.
- The price variance should be the same across both groups.
- Each property listing is separate; no listing affects another.

# 8. Data Preparation
Right now, the price and size columns are stored as strings. So first, we have to strip out non-numeric symbols (commas, currency signs), then convert these fields to floats.  
We’ll filter the data so it only covers listings in our two target cities.  
There are 539 listings with missing prices; we’ll either drop them or fill them in, depending on what makes sense.

# 9. Analysis Steps
- Start with the basics: mean, standard deviation, and median for each city.
- Next, draw histograms and boxplots; these help spot outliers or odd distribution shapes.
- Then, run the t-test and take a close look at the p-value.

# 10. Expected Outcome
We expect to reject the null hypothesis. Because New Cairo is close to the new capital and loaded with luxury developments, we expect its average property prices to be higher than Sheikh Zayed’s.

# 11. Conclusion
The results will tell us if location really drives the price gap in Egypt’s residential market. That insight should help both investors and city planners make smarter decisions.

# 12. Tools & Infrastructure
**Language:** Python (Pandas & SciPy)  
**Visualization:** Matplotlib & Seaborn  
**Environment:** Google Colab  
**Version Control:** GitHub repo: [Yalla-Nanalyz] (https://github.com/oppadmaged/Yalla-Nanalyze-Data-Analysis-Project-III)
