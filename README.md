## **World Happiness Analysis: Does Wealth Guarantee Well-being?**
_DSCP Final Project | William | Candice_

### **1. Project Overview**

This project explores the correlation between a country's economic output (GDP per Capita) and its citizens' self-reported happiness scores. By analyzing global datasets, I aim to determine if financial strength is the primary driver of national well-being or if regional factors play a more significant role.

### **2. Objectives**

- Analyze Correlation: Quantify the relationship between GDP and Happiness.
- Regional Benchmarking: Identify which global regions lead in happiness relative to their economic status.
- Data Transformation: Categorize countries into distinct income levels to observe macro-trends.

### **3. Dataset & Pre-processing**

- Source: Inspired by the World Happiness Report.
- Cleaning: Implemented automated logic to detect missing values and fill them with column means to prevent statistical bias.
- Engineering: Created a custom categorical feature (Income_Level) to segment data into "High Income" and "Low/Medium Income."

### **4. Methodology (Algorithm & Pseudocode)**
To ensure transparency in the analysis, the project follows this logical flow:

1. Ingestion: Load global happiness data into a Pandas DataFrame.
2. Cleanse: Identify and fill null values.
3. Algorithm (Categorization): Apply a threshold logic ($GDP > 1.0$) to define income brackets.
4. Aggregation: Group results by Region to find the mean happiness score.
5. Visualization: Generate comparative plots using Seaborn and Matplotlib.

### **5. Key Findings & Visualizations**

<img width="833" height="549" alt="Image" src="https://github.com/user-attachments/assets/00fd81b9-b9f9-4e30-8da9-745a0e767a15" />
<img width="957" height="549" alt="Image" src="https://github.com/user-attachments/assets/4ac9632b-207c-456b-9d0a-54309b7d1f0c" />

**A. Economic Correlation**
The scatter plot reveals a strong positive trend. As GDP per Capita increases, there is a visible rise in Happiness Scores, confirming that economic stability is a foundational requirement for high well-being.
**B. Regional Rankings**
Europe and North America consistently show the highest happiness averages, while Sub-Saharan Africa shows the lowest, correlating with the regional GDP averages.

### **6. Conclusion (Final Analysis)**
Based on the data, there is a clear "income floor" for happiness; countries with a GDP per capita above 1.0 rarely report happiness scores below 6.5. However, the variance in middle-income countries suggests that while money is a major factor, it is not the only factor. Social safety nets and regional stability likely account for the outliers in the data.
