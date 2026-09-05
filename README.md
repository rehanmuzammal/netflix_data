# Netflix Content Analysis — Power BI Dashboard

A Power BI project analyzing Netflix's content library — covering data preparation, content overview, global distribution insights, and growth trends over time.

## 📊 Project Overview

This project uses a Netflix content dataset (`Dataset.csv`) containing details such as title, type (Movie/TV Show), director, country, date added, release year, rating, duration, and genre (`listed_in`). The project is broken into four tasks, each building a dedicated Power BI report page.

---

## Task 1 (Easy) — Data Preparation & Power BI Setup

**Description:** Import, clean, and transform Netflix data to prepare it for reporting and visualization.

**Workflow:**
- Imported the dataset into Power BI
- Cleaned and transformed data using Power Query (replaced missing `director` values, converted `date_added` to Date type, split `duration` into value/unit, split `listed_in` into individual genre rows)
- Handled missing values and checked for duplicates
- Created a Date table and relationships
- Validated data accuracy

**Skills:** Power BI Fundamentals, Power Query Editor, Data Transformation, Data Modeling

![Task 1 Screenshot] https://github.com/rehanmuzammal/netflix_data/blob/main/Dashbord%20Overview.png

## Task 2 (Easy) — Netflix Content Overview Dashboard

**Description:** An interactive dashboard displaying Netflix content distribution and key metrics.

**Workflow:**
- Defined KPIs: Total Content, Total Movies, Total TV Shows, Total Countries, Total Genres (via DAX measures)
- Built KPI cards, a genre bar chart, a country column chart, and a Movies vs TV Shows donut chart
- Added slicers for release year, country, and type
- Optimized the dashboard layout

**Skills:** Dashboard Development, Visual Design, KPI Reporting, Data Storytelling

![Task 2 Screenshot] https://github.com/rehanmuzammal/netflix_data/blob/main/Dashbord%20Overview.png

## Task 3 (Medium) — Global Content Insights Dashboard

**Description:** Analyze Netflix content distribution across countries and regions.

**Workflow:**
- Created country-level metrics (Total Countries, Avg Content Per Country)
- Built a geographic view (Matrix table ranking countries by content volume)
- Added a drill-down bar chart (Country → Genre)
- Implemented interactive filters (release year, type)
- Highlighted the top content-producing country

**Skills:** Map Charts, Drill-Down Reports, Geographic Analytics, Business Intelligence

![Task 3 Screenshot] https://github.com/rehanmuzammal/netflix_data/blob/main/Global%20Insight.pngs

## Task 4 (Medium) — Content Growth & Trend Analysis

**Description:** Develop a dashboard to analyze Netflix content growth over time.

**Workflow:**
- Analyzed release trends with a year-wise line chart
- Compared Movies vs TV Shows growth over time
- Tracked content growth with an area chart
- Added trend lines for growth indicators
- Generated growth insights (e.g., latest year content volume)

**Skills:** Trend Visualization, DAX Basics, Time Intelligence, Analytical Reporting

![Task 4 Screenshot]https://github.com/rehanmuzammal/netflix_data/blob/main/Screenshot%202026-09-06%20012811.png

- Power BI Desktop

**Power Query Editor (Data Cleaning & Transformation):**
- Replace Values (handling missing `director` entries)
- Change Data Type (converting `date_added` to Date)
- Split Column by Delimiter (splitting `duration` into value/unit; splitting `listed_in` into individual genre rows)
- Column Quality & Column Distribution view (checking for blanks/nulls)
- Remove Duplicates

**Data Modeling:**
- Custom Date Table (`CALENDAR` function)
- Relationships between tables (Modeling / Model view)

**DAX (Data Analysis Expressions) — Measures:**
- `DISTINCTCOUNT` — Total Content, Total Countries, Total Genres
- `CALCULATE` — Total Movies, Total TV Shows, Top Country
- `DIVIDE` — Avg Content Per Country
- `RANKX` — Top Country Rank
- `TOPN`, `VALUES`, `ALL`, `MAX` — Top Country / latest year insights

**Visualizations Built:**
- Card (KPIs)
- Clustered Bar Chart / Clustered Column Chart
- Donut Chart
- Matrix Table (country ranking, used as a Map alternative)
- Line Chart & Area Chart (trend analysis, with trend lines)
- Slicers (release year, country, type)

## 📁 Repository Contents
- `Dataset.csv` — source dataset
- `Netflix_Dashboard.pbix` — Power BI project file
- `screenshots/` — dashboard screenshots for each task

## 🚀 How to Use
1. Download `Netflix_Dashboard.pbix`
2. Open it in Power BI Desktop
3. Explore each report page: Overview, Global Insights, Trend Analysis
