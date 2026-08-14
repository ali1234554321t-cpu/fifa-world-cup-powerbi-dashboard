# 🏆 FIFA World Cup Power BI Dashboard

An interactive **FIFA World Cup Dashboard** built using **Microsoft Power BI** to analyze and visualize team performance across World Cup tournaments.

The dashboard allows users to explore overall World Cup statistics and drill down into individual teams such as **Germany, France, Brazil, Argentina, Egypt, Portugal, Italy, Algeria, Nigeria**, and others.

---

## 📊 Dashboard Overview

The dashboard provides insights into:

* 🌍 Team participation
* 🏟️ Games played
* 🏆 Wins
* ❌ Losses
* 🤝 Draws
* ⚽ Goals For
* 🥅 Goals Against
* 📈 Goal Difference
* 🎯 Points
* 📅 Years participated
* 📊 Points achieved per year
* ⚽ Goals For vs Goals Against
* 📌 Win / Loss / Draw distribution
* 🔎 Team-level performance analysis

---

## 🖥️ Dashboard Pages

### 1. World Cup Overview

The main dashboard provides an overall comparison between participating teams.

It includes:

* Team ranking table
* Games played
* Wins, losses, and draws
* Goals scored and conceded
* Goal difference
* Total points
* Years participated
* Highest scoring team
* Lowest scoring team
* Goals scored per World Cup year

---

### 2. Team Analysis

The dashboard also provides a detailed view for an individual team.

After selecting a team, the dashboard dynamically updates all visuals.

The team page contains:

* Team information
* National flag
* World Cup participation years
* Games played
* Wins
* Losses
* Draws
* Goals scored
* Goals against
* Goal difference
* Points
* Points achievement per year
* Goal involvement
* Goals For vs Goals Against
* Win / Loss / Draw analysis

---

## 🔄 Interactive Features

The dashboard uses Power BI interactive features to make the analysis dynamic.

Users can:

1. Select a country.
2. View the selected team's statistics.
3. Analyze the years in which the team participated.
4. Compare goals scored and goals conceded.
5. Analyze wins, losses, and draws.
6. Track points achieved across tournaments.

All visuals respond dynamically to the selected team.

---

## 🛠️ Tools & Technologies

* **Microsoft Power BI**
* **Power Query**
* **DAX**
* **Data Modeling**
* **Data Visualization**

---

## 🔧 Data Preparation Process

The project followed a complete data analysis workflow:

### Step 1 — Data Collection

The FIFA World Cup dataset was collected and prepared for analysis.

### Step 2 — Data Cleaning

The data was cleaned and transformed using **Power Query**.

Main tasks included:

* Removing unnecessary columns
* Handling missing values
* Correcting data types
* Preparing team and tournament information
* Creating fields required for analysis

### Step 3 — Data Modeling

The cleaned data was loaded into Power BI and prepared for analysis.

The model was structured to support:

* Team-level analysis
* Tournament-level analysis
* Year-based analysis
* Performance calculations

### Step 4 — DAX Calculations

DAX measures were created to calculate important KPIs such as:

* Games Played
* Wins
* Losses
* Draws
* Goals For
* Goals Against
* Goal Difference
* Points
* Team Participation

Example calculations:

```DAX
Games Played =
COUNTROWS('WorldCup')
```

```DAX
Total Wins =
CALCULATE(
    COUNTROWS('WorldCup'),
    'WorldCup'[Result] = "Win"
)
```

```DAX
Total Losses =
CALCULATE(
    COUNTROWS('WorldCup'),
    'WorldCup'[Result] = "Loss"
)
```

```DAX
Total Draws =
CALCULATE(
    COUNTROWS('WorldCup'),
    'WorldCup'[Result] = "Draw"
)
```

```DAX
Goal Difference =
[Total Goals For] - [Total Goals Against]
```

```DAX
Points =
([Total Wins] * 3) + [Total Draws]
```

> Note: The exact DAX formulas may vary depending on the structure and column names of the original dataset.

---

## 📈 Visualization Process

After preparing the data and creating the required measures, different Power BI visuals were used to communicate the insights.

### Main Visuals

* Tables
* Cards
* Line Charts
* Donut Charts
* Treemap
* Slicers
* KPI-style visuals

The visuals were designed to provide both an overall World Cup analysis and detailed team-level insights.

---

## 🎯 Key Insights

The dashboard can be used to answer questions such as:

* Which teams have the most World Cup wins?
* Which teams participated in the most tournaments?
* Which team scored the most goals?
* Which teams have the highest number of losses?
* How many points did a team achieve?
* How did a team's performance change over different tournaments?
* How many goals did a team score compared to the goals it conceded?
* Which years did a specific team participate in?

---

## 📂 Project Structure

```text
fifa-world-cup-powerbi-dashboard/
│
├── README.md
│
├── Dashboard/
│   └── FIFA_World_Cup_Dashboard.pbix
│
├── Screenshots/
│   ├── world-cup-overview.png
│   ├── france-analysis.png
│   ├── nigeria-analysis.png
│   ├── egypt-analysis.png
│   ├── portugal-analysis.png
│   ├── italy-analysis.png
│   └── germany-analysis.png
│
└── Data/
    └── world-cup-data.csv
```

---

## 🚀 How to Use

1. Download or clone this repository.
2. Open the `.pbix` file using **Microsoft Power BI Desktop**.
3. Use the country/team selector to choose a team.
4. Explore the interactive visuals and KPIs.
5. Analyze the team's World Cup performance.

---

## 📸 Dashboard Preview

### World Cup Overview

![World Cup Overview](Screenshots/world-cup-overview.png)

### Team Analysis

![France Analysis](Screenshots/france-analysis.png)

![Germany Analysis](Screenshots/germany-analysis.png)

![Egypt Analysis](Screenshots/egypt-analysis.png)

---

## 👨‍💻 Project Author

**Ali Rabea**

Data Analyst | Power BI | SQL | Python | Excel

---

## ⭐ Project Purpose

This project was created as a **Data Analytics and Power BI portfolio project** to demonstrate skills in:

* Data Cleaning
* Data Transformation
* Data Modeling
* DAX
* Data Visualization
* Interactive Dashboard Design
* Business/Data Storytelling


