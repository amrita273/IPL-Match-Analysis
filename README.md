# 🏏 IPL Match Analysis (2008-2022)

Exploratory Data Analysis on Indian Premier League match data 
spanning 15 seasons. This project was built to practice data 
cleaning, analysis and visualization using Python and Power BI.

---

## 📊 What I Analyzed

- Most successful teams by total wins
- Does winning the toss actually help win the match?
- Bat vs Field — what do captains prefer after winning toss?
- Top 10 Player of the Match award winners
- Season-wise total matches played over the years
- Top host cities by number of matches
- Biggest wins by run margin
- How matches were won — by runs vs by wickets

---

## 🛠️ Tools Used

- Python
- Pandas — data cleaning and analysis
- Matplotlib — data visualization
- Jupyter Notebook / Google Colab
- Power BI — interactive dashboard

---

## 📁 Dataset

- Source: [Kaggle IPL Dataset](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020)
- File used: `matches.csv`
- Total matches: ~950 across 15 seasons

---

## 🧹 Data Cleaning Done

- Dropped 5 no-result matches where winner was null
- Filled missing city values with 'Unknown'
- Filled missing player_of_match with 'Unknown'
- Filled result_margin, target_runs, target_overs nulls with 0
- Filled method column nulls with 'Normal' since most matches
  don't use DLS or any special method

---

## 📌 Key Findings

- Mumbai Indians have the most IPL wins overall
- Captains prefer fielding first after winning the toss
- Winning the toss does NOT guarantee winning the match
- Mumbai and Kolkata are the most frequent host cities

---

## 📊 Power BI Dashboard

Built an interactive dashboard on the same dataset after 
completing the Python analysis.

### Visuals Built
- Bar Chart — Total wins by each team
- Pie Chart — Toss decision preference (bat vs field)
- Line Chart — Number of matches played per season
- Map Visual — Matches hosted across Indian cities
- Card Visuals — 3 KPI cards showing:
  - Total matches played
  - Total seasons covered
  - Most successful team

### Interactivity Added
- Slicer by Season — filter entire dashboard by year
- Slicer by Team — see stats for any specific team

### Steps Followed
1. Imported the cleaned `matches.csv` directly into Power BI
2. Used Power Query to verify data types were correct
3. Created calculated measures using DAX for win counts
4. Designed the layout with slicers on the left panel
5. Published the report

### DAX Measure Used
