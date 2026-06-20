Netflix Content Analytics Dashboard

📊 An interactive Power BI dashboard designed to analyze Netflix's content library using IMDb ratings, audience engagement metrics, content classifications, and release trends.

Project Overview

This project provides insights into Netflix's content catalog by analyzing:

Content distribution (Movies vs TV Shows)
Content quality based on IMDb ratings
Audience age certifications
Netflix content growth trends
Top-rated titles
Content engagement using IMDb votes

The dashboard was developed using Power BI, Power Query, and DAX to transform raw data into actionable business insights.

Objectives
Analyze Netflix's content portfolio
Evaluate content quality using IMDb ratings
Identify audience targeting through age certifications
Track content growth over time
Highlight top-performing titles
Present insights through an executive-level dashboard

| Metric              | Value       |
| ------------------- | ----------- |
| Total Titles        | 5,628       |
| Movies              | 3,000+      |
| TV Shows            | 2,000+      |
| Total IMDb Votes    | 123 Million |
| Average IMDb Rating | 6.53        |

Data Cleaning & Transformation

Performed using Power Query:

Removed duplicate records
Handled null and missing values
Filtered invalid records
Created custom Rating Categories
Standardized data types
Generated calculated columns for analysis.

DAX Measures Used
Total Titles = COUNT(Netflix[title])

Total Movies =
CALCULATE(
    COUNT(Netflix[title]),
    Netflix[type] = "MOVIE"
)

Total Shows =
CALCULATE(
    COUNT(Netflix[title]),
    Netflix[type] = "SHOW"
)

Average IMDb =
AVERAGE(Netflix[imdb_score])

Total Votes =
SUM(Netflix[imdb_votes])

Dashboard Features

✅ Executive KPI Cards

✅ Content Quality Distribution

✅ Content Type Distribution

✅ Netflix Content Growth Trend

✅ Top Rated Titles Ranking

✅ Audience Age Certification Analysis

✅ Interactive Filtering

✅ Business Insights Panel.

Key Insights
Movies represent approximately 64.5% of Netflix's content catalog.
The average IMDb score across all titles is 6.53.
Only 9.6% of titles fall into the Excellent rating category.
Netflix experienced rapid catalog expansion after 2015.
TV-MA is the most common age certification.
A significant portion of content lacked age certification metadata.

Tools & Technologies
Power BI
Power Query
DAX
Data Visualization
Data Cleaning
Business Intelligence
Dashboard Design

Dashboard Preview
<img width="1420" height="798" alt="Screenshot 2026-06-20 115552" src="https://github.com/user-attachments/assets/34b318da-856e-463c-93f7-d347d078aef7" />


Author

Kaustubh Kulkarni

Power BI | SQL | Python | Data Analytics
