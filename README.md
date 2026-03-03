🌾 Sugarcane Production Analysis Project
📌 Project Overview

This project analyzes global sugarcane production by exploring key factors such as:

🌍 Production volume

🌱 Land usage (Acreage)

📈 Yield per hectare

👥 Production per person

Through comprehensive Exploratory Data Analysis (EDA), we identify top-producing countries and continents, examine relationships between variables, and visualize global production distribution.

The insights gained can help inform agricultural strategies and improve resource management in the sugarcane industry.

📂 Dataset

Dataset: List of Countries by Sugarcane Production

Includes country-wise production metrics and continent classification.

🧹 Data Cleaning

Before analysis, the dataset was cleaned to ensure accuracy and usability.

1️⃣ Removing Unwanted Characters

Removed periods (.) from:

Production (Tons)

Acreage (Hectare)

Replaced commas with periods in:

Production per Person (Kg)

Standardized decimal formats for numerical computations.

2️⃣ Removing Unnecessary Columns

Dropped irrelevant columns such as:

Unnamed: 0

Used drop(axis=1) for column removal.

3️⃣ Renaming Columns

Renamed columns for consistency and easier access:

Production (Tons) → Production(Tons)

Production per Person (Kg) → Production_per_person(Kg)

Other columns standardized similarly.

4️⃣ Handling Missing Values
Missing Values Found:
Country                      0
Continent                    0
Production(Tons)             0
Production_per_person(Kg)    0
Acreage(Hectare)             1
Yield(Kg/Hectare)            1
Action Taken:

Dropped rows with missing values in:

Acreage(Hectare)

Yield(Kg/Hectare)

Reset index for clean dataset.

5️⃣ Data Type Conversion

Converted relevant columns to float type:

Production(Tons)

Production_per_person(Kg)

Acreage(Hectare)

Yield(Kg/Hectare)

📊 Exploratory Data Analysis (EDA)
🔍 Univariate Analysis
1️⃣ Countries Producing Sugarcane by Continent
Africa           38
Asia             25
North America    22
South America    11
Oceania           4
Europe            2

📌 Africa has the highest number of sugarcane-producing countries.

2️⃣ Distribution of Key Variables

Histograms were used to analyze:

Production (Tons)

Production per Person (Kg)

Acreage (Hectare)

Yield (Kg/Hectare)

Key Observations:

Production(Tons): Highly skewed due to Brazil, India, and China.

Production per Person: Skewed distribution.

Acreage: Moderate skewness.

Yield: Varies significantly by farming efficiency.

3️⃣ Outlier Detection (Boxplots)

Boxplots revealed:

Major production outliers: Brazil, India, China

High-yield outliers indicating efficient farming nations

4️⃣ Violin Plot (Production)

Wide spread distribution

Strong right skew

Few dominant producing countries

🔗 Bivariate Analysis
1️⃣ Highest Acreage Countries

Top 15 countries show:

Brazil

India

China

These dominate land usage for sugarcane.

2️⃣ Highest Yield per Hectare

🇬🇹 Guatemala has the highest yield

Indicates strong agricultural efficiency

3️⃣ Highest Production per Person

🇵🇾 Paraguay leads in production relative to population

4️⃣ Correlation Analysis

Correlation Matrix Results:

Variables	Correlation
Production vs Acreage	0.997 (Strong Positive)
Production vs Yield	0.132 (Weak Positive)

📌 Insight:
Land size strongly determines production, not yield efficiency.

Heatmap used for visualization.

5️⃣ Acreage vs Production

Scatter plot confirms:

Larger land area → Higher total production

6️⃣ Yield vs Production

Higher yield does NOT always mean higher total production

Land size plays a more significant role

🌍 Continental Analysis
1️⃣ Production by Continent

Total Production Ranking:

🥇 South America

🥈 Asia

🥉 Africa

South America leads due to Brazil's dominance.

2️⃣ Does Number of Countries Affect Production?

Key Insight:

More countries ≠ Higher production

South America has fewer countries but high production

Dominance of Brazil drives total output

📈 Key Insights

Land area is the strongest predictor of total production.

Production is heavily concentrated in a few countries.

Yield efficiency does not always translate to highest total output.

Geographic distribution varies significantly across continents.

🛠 Tools Used

Python

Pandas

NumPy

Matplotlib

Seaborn

🚀 Conclusion

This project demonstrates:

End-to-end data cleaning

Statistical exploration

Visualization techniques

Correlation analysis

Insight generation from real-world agricultural data

It highlights how data-driven analysis can support agricultural planning and resource optimization.
