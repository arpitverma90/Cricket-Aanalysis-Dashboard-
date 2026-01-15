# 🏏 Cricket Analysis Dashboard | End-to-End Power BI Analytics Project

## 📌 Project Summary

This project is a **complete end-to-end cricket analytics solution** built using raw **JSON match data**, transformed through **Python (Google Colab)**, and visualized using **Power BI** with a strong focus on **data modeling, DAX measures, and analytical storytelling**.

The dashboard provides **deep insights into batting performance, bowling efficiency, and match outcomes**, replicating how real-world sports or business analytics platforms are designed—from raw ingestion to decision-ready dashboards.

---

## 🎯 Objective of the Project

* Convert **unstructured JSON cricket data** into a clean analytical dataset
* Apply **data engineering and transformation logic** using Python
* Build a **scalable Power BI data model**
* Design **calculated measures and calculated columns** using DAX
* Create a **professional analytics dashboard** suitable for portfolio and interviews

---

## 📂 Data Sources

The dataset consists of multiple JSON files containing:

* Batting summaries (runs, balls, boundaries, strike rate, dismissals)
* Bowling summaries (overs, balls, wickets, economy, runs conceded)
* Match results (teams, winners, margins, venues, dates)
* Player metadata (team, batting style, bowling style, role)

These JSON files contain **nested and semi-structured data**, requiring transformation before analysis.

---

## 🔄 Data Engineering & Transformation (Python – Google Colab)

### Key Transformation Steps:

* Loaded raw JSON files into Python
* Flattened nested structures using dictionaries and loops
* Converted string-based numeric fields into integers/floats
* Standardized column names and formats
* Split data into logical entities (batting, bowling, match, player)
* Exported cleaned datasets as **CSV files** for BI consumption

This step simulates a **real-world ELT pipeline**, where raw data is prepared before analytics.

---

## 🧩 Data Modeling in Power BI

### Tables Used:
The Power BI model is built using the following fact and dimension tables:
🔹 Dimension Tables
•	dim_match_summary
o	Match date, teams, venue, winner, result margin
•	dim_players
o	Player name, team, batting style, bowling style, role
•	dim_players_no_images
o	Lightweight player dimension used for performance optimization
🔹 Fact Tables
•	fact_batting_summary
o	Runs, balls faced, boundaries, strike rate, dismissals, batting position
•	fact_bowling_summary
o	Balls bowled, runs conceded, wickets, economy-related attributes


### Modeling Approach:

* Fact-dimension style layout
* Relationships created on match and player keys
* Measures separated into a **dedicated Key Measures table**
* Minimal calculated columns; logic pushed into DAX measures where possible

This approach ensures:

* Better performance
* Cleaner visuals
* Reusable business logic

---

## 📐 DAX Measures & Calculated Columns

All calculations are **explicitly documented in an Excel file** included in the repository.

### 🟦 Batting Measures

* **Total Runs**
* **Total Innings Batted**
* **Total Innings Dismissed**
* **Batting Average**
* **Total Balls Faced**
* **Strike Rate**
* **Average Batting Position**
* **Boundary Percentage**
* **Average Balls Faced per Innings**

### 🟩 Bowling Measures

* **Total Wickets**
* **Total Balls Bowled**
* **Total Runs Conceded**
* **Bowling Economy**
* **Bowling Strike Rate**

Each measure:

* Uses `SUM`, `COUNT`, `AVERAGE`, and `DIVIDE`
* Includes error handling (division by zero)
* Is filter-aware and slicer-responsive

---

## 📊 Dashboard Features & Insights

* Player-level batting and bowling performance
* Strike rate vs average comparisons
* Economy and wicket efficiency analysis
* Match-wise and team-wise breakdowns
* Interactive filtering using slicers
* Clean and minimal visual design for clarity

The dashboard enables **quick performance comparisons** and **data-driven cricket insights**.

---

## 🖼️ Dashboard Snapshots (GitHub Preview)

Below are snapshots of the Power BI dashboard showcasing key analytics views.

### 🔹 Overall Dashboard View

<img width="1307" height="731" alt="image" src="https://github.com/user-attachments/assets/dca762a2-78d4-41ab-8a85-4f085f25895a" />


### 🔹 Batting Performance Analysis

<img width="1303" height="733" alt="image" src="https://github.com/user-attachments/assets/d129caee-4b3d-448f-adab-981fdd209118" />


### 🔹 Bowling Performance Analysis

<img width="1308" height="727" alt="image" src="https://github.com/user-attachments/assets/e452e72d-fc0a-4db2-89bc-19cff003a8f1" />


## 📁 Repository Structure

| Path / File                                  | Type             | Description                                                                                                                 |
| -------------------------------------------- | ---------------- | --------------------------------------------------------------------------------------------------------------------------- |
| `data/`                                      | Folder           | Contains cleaned and transformed CSV datasets generated from raw JSON files                                                 |
| `data/batting_summary.csv`                   | CSV              | Ball-by-ball aggregated batting data including runs, balls faced, boundaries, strike rate, dismissals, and batting position |
| `data/bowling_summary.csv`                   | CSV              | Bowling performance data containing overs, balls bowled, runs conceded, wickets, and economy-related attributes             |
| `data/match_results.csv`                     | CSV              | Match-level details such as teams, match date, venue, winner, and result margin                                             |
| `data/player_info.csv`                       | CSV              | Player metadata including team, batting style, bowling style, and playing role                                              |
| `notebooks/`                                 | Folder           | Contains Python notebooks used for data transformation and preprocessing                                                    |
| `notebooks/json_to_csv_transformation.ipynb` | Jupyter Notebook | Parses raw JSON files, flattens nested structures, cleans data types, and exports analysis-ready CSV files                  |
| `dashboard/`                                 | Folder           | Contains Power BI dashboard and related analytical assets                                                                   |
| `dashboard/Cricket Analysis Dashboard.pbix`  | Power BI File    | Interactive Power BI dashboard built on fact–dimension modeling and DAX-based measures                                      |
| `DAX-Measures-and-Calculated-Columns.xlsx`   | Excel            | Complete documentation of all DAX measures and calculated columns, including formulas, purpose, and source tables           |
| `README.md`                                  | Markdown         | Project documentation explaining objectives, data pipeline, data model, measures, and dashboard insights                    |


## 🛠️ Tools & Technologies Used

* Python (Google Colab)
* JSON Data Handling
* Power BI
* DAX (Measures & Calculated Columns)
* Data Modeling & Analytics Design

---

## 🚀 Key Takeaways

* Demonstrates **end-to-end analytics workflow**
* Strong focus on **DAX logic and data modeling**
* Real-world style data engineering using Python
* Portfolio-ready BI dashboard with documentation

---

## 📌 Future Enhancements

* Tournament-level trend analysis
* Player ranking system
* Win probability metrics
* Advanced visuals using tooltips and drill-through pages

<<<<<<< HEAD

=======
>>>>>>> da48f3df324be4ce3cf98dccccc8559b9a8b8f74
