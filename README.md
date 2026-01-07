**Methodology & Technical Approach**
This project applies a full data analytics and forecasting pipeline to large-scale, real-world crime data from Los Angeles (2020–2025), with an emphasis on data integrity, temporal analysis, and predictive modeling.

**Data Acquisition & Integration**
Crime incident records were sourced from the LAPD public crime dataset and augmented with macroeconomic indicators from the Federal Reserve Bank of St. Louis (FRED). External datasets were time-aligned to ensure consistency across analytical stages.

**Data Cleaning & Transformation**
The raw dataset required substantial preprocessing due to missing values, redundant fields, and ambiguous metadata. Columns with excessive null values or low analytical relevance were removed. Remaining missing values were handled using context-appropriate placeholders. Categorical variables were standardized, and additional derived features—such as crime categories and victim age groups—were engineered to support deeper analysis.

**Exploratory Analysis**
Exploratory Data Analysis (EDA) was conducted to identify temporal, spatial, and behavioral crime patterns. This included:

- Long-term and seasonal crime trends
- Crime distribution by type, region, and location
- Day-of-week and time-of-day analysis
- Demographic patterns related to victim characteristics

Visual analytics were used extensively to validate trends and expose inconsistencies in reporting.

**Economic Relationship Analysis**
Unemployment data from FRED was incorporated to assess the relationship between economic conditions and crime rates. Correlation analysis revealed a negative relationship between unemployment and reported crime, particularly during the COVID-19 period, highlighting the impact of mobility restrictions and economic disruption on crime patterns.

**Anomaly Detection & Data Reliability**
Significant anomalies were detected in late-2024 and 2025 data due to LAPD reporting system changes. These periods were explicitly flagged and treated cautiously in downstream analysis. Heatmaps and temporal comparisons were used to validate reporting gaps and structural breaks.

**Forecasting & Predictive Modeling**
Two time-series forecasting approaches were implemented:

- ARIMA for long-term, yearly crime projections (excluding incomplete 2025 data)
- Prophet for short-term, monthly forecasts incorporating recent trends

Forecast outputs were evaluated in the context of data quality limitations and reporting delays.

**Visualization & Interpretation**

Results were communicated through clear, interpretable visualizations including trend plots, heatmaps, and forecast confidence intervals. All findings were consolidated into a formal analytical report with documented assumptions and limitations.

**Technical Focus**
- Real-world data cleaning and validation
- Time-series analysis under incomplete data conditions
- Integration of external economic indicators
- Forecasting with uncertainty awareness
- Analytical storytelling through visualization
