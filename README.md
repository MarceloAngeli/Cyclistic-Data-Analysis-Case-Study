# Cyclistic-Data-Analysis-Case-Study
## Google Data Analyst Professional Certificate Capstone.

> **AVISO:** Clique [aqui](https://github.com/MarceloAngeli/Cyclistic-Data-Analysis-Case-Study/blob/main/README.pt.md) para obter a versão do READme em Português.

### 1. Introduction

This project is a case study conducted as the capstone for the Google Data Analyst Professional Certificate. The analysis focuses on the bike-share usage data from a fictional company, Cyclistic, to understand the key differences between its two customer segments: casual riders and annual members. The ultimate goal is to provide data-driven recommendations for a marketing campaign aimed at converting casual riders into more profitable annual members. 

### 2. The Business Task

The Director of Marketing has tasked the data analytics team with answering the following key question: **What are the main differences in vehicle usage between members and
casual riders?**. The insights derived from this analysis will be used to shape a new marketing strategy designed to increase the conversion rate of casual riders to annual members, as annual memberships are significantly more profitable for the company.

### 3. Data Source

The dataset used for this analysis is real-world trip data from the Chicago-based bike-share company Divvy. For the purpose of this case study, this data is treated as if it belongs to Cyclistic. The dataset spans 12 months, from July 2024 to June 2025, and contains information on individual trips, including start/end times, start/end station locations, user type, and vehicle type.

* The data can be accessed [here](https://divvy-tripdata.s3.amazonaws.com/index.html).

### 4. Tools Used

* **R & RStudio:** For data cleaning, transformation, and analysis.
* **R Packages:**
    * `tidyverse`: For general data manipulation and wrangling.
    * `ggplot2`: For creating data visualizations.
    * `scales`: For formatting visualization scales.

### 5. The Analysis Process

The analysis followed the six steps of the data analysis framework: **Ask, Prepare, Process, Analyze, Share, and Act.**

1.  **Prepare:** Data from 12 separate `.csv` files (one for each month) was gathered, assessed for consistency, and merged into a single comprehensive dataframe.
2.  **Process:** The data was thoroughly cleaned to ensure integrity. This included:
    * Creating new columns for analysis, such as trip duration, month, and day of the week.
    * Removing trips with negative duration.
    * Removing duplicate entries.
    * Validating that categorical columns contained only expected values.
3.  **Analyze:** The cleaned data was analyzed to identify key trends and differences between casual riders and members.
4.  **Share & Act:** Key findings were visualized using `ggplot2`, and a final set of actionable recommendations was developed based on these insights.

### 6. Key Findings

The analysis revealed several clear behavioral differences between the two customer segments:

* **Seasonality and Day-of-Week Usage:**
    * Annual members use the service consistently throughout the year, with a slight increase in summer. Their usage is highest on weekdays, suggesting a pattern of commuting to and from work.
    * Casual riders are highly seasonal, with usage peaking dramatically in the warm months (June-October). They overwhelmingly prefer to ride on weekends (Saturdays and Sundays), indicating recreational use.

* **Trip Duration:**
    * Casual riders take significantly longer trips on average, at approximately 24 minutes per ride.
    * Annual members take shorter, more direct trips, with an average duration of about 13 minutes.

* **Vehicle Preference:**
    * Both groups show a strong preference for electric bikes over classic bikes.
    * The preference for electric vehicles is even more pronounced among casual riders.

### 7. Recommendations

Based on the findings, the following recommendations are proposed for the marketing campaign:

1.  **Target Marketing on Weekends During Peak Season:** Focus advertising efforts on Saturdays and Sundays between spring and summer (June-November), when casual riders are most active.
2.  **Promote Commuter Benefits:** Create campaigns highlighting the cost-effectiveness and convenience of an annual pass for daily commuting, targeting potential customers during weekdays.
3.  **Feature Electric Bikes in Advertisements:** Since electric bikes are highly popular with casual riders, marketing materials should prominently feature these vehicles to capture their interest.
4.  **Create Conversion-Focused Promotions:** Offer incentives like a "Weekend Pass" that could roll into a discounted annual membership, or promotions targeting users who take longer, recreational-style trips.

### 8. Repository Contents

* **`Cyclistic_Case_Study_English_Version.pdf`:** The final, detailed report of the case study including visualizations and a narrative of the findings.
* **`Cyclistic_Case_Study_English_Version.Rmd`:** The R Markdown file containing all the code used for data cleaning, analysis, and visualization.
* **`README.en.md`:** This explanatory file.
