# 📊 ElectViz – Election Data Visualization for Media

ElectViz is an interactive Power BI project designed to analyze election results across multiple years (2009, 2014, 2019) and present them in a structured, media-style dashboard format.

This project transforms raw election data into meaningful visual insights using data modeling, DAX calculations, and interactive visualizations across **5 dedicated dashboards**.

---

## 📌 Project Objectives

- Provide a high-level summary of election results via an overview dashboard
- Analyze historical election trends across 2009, 2014,and 2019
- Simulate a real-time election results dashboard with dynamic year filtering
- Identify leading parties and winning candidates based on constituencies won
- Visualize seat distribution and vote share across parties
- Analyze voter turnout and regional participation patterns
- Surface party and candidate-level insights using advanced visuals

---

## 🗂 Dataset Description

The dataset covers Indian general election results for three years — **2009, 2014, and 2019** — with the following fields:

| Field | Description |
|---|---|
| **Year** | Election year (2009, 2014, or 2019) |
| **Constituency** | Name of the parliamentary constituency |
| **Candidate** | Candidate's name |
| **Party** | Political party the candidate represents |
| **Votes** | Total votes received by the candidate |
| **Turnout %** | Voter turnout percentage for the constituency |
| **Total Electors** | Total registered electors in the constituency |

---

## 📊 Dashboards Overview

The report contains **5 interactive dashboard pages**, each serving a distinct analytical purpose.

---

### 1️⃣ Election Overview

A high-level summary dashboard that gives a quick snapshot of the entire election dataset.

**Key Visuals:**

| Visual | Description |
|---|---|
| 🃏 **KPI Cards** | Total Votes Cast, Total Electors, Total Constituencies, Total Parties |
| 🥧 **Pie Chart** | Party-wise vote share distribution |
| 📋 **Results Table** | Constituency, Candidate, Party, and Votes for all records |
| 📈 **Column Chart** | Turnout % by Constituency |
| 📈 **Clustered Column Chart** | Total votes by Year |

**Purpose:**
To provide an at-a-glance summary of election scale, participation, and party vote share across all years.

---

### 2️⃣ Historical Trends

This dashboard focuses on long-term analysis, showing how elections have evolved across 2009, 2014, and 2019.

**Key Visuals:**

| Visual | Description |
|---|---|
| 📉 **Line & Column Combo Chart** | Voting & Turnout Trends Over Time — overlays total votes (columns) with average turnout % (line) by year |
| 📈 **Clustered Column Chart** | Party Vote Comparison by Year — compares party-wise votes across election cycles |
| 📊 **Clustered Bar Chart** | Constituency-wise Turnout Change — shows per-constituency turnout variation across years |
| 📊 **Clustered Bar Chart** | Top 5 Constituencies by Vote Growth — ranks constituencies with the highest vote growth % |
| 📉 **Line Chart** | Average Turnout trend across election years |
| 🗺️ **Map** | Geographical Vote Distribution — plots constituencies on a map with vote count and turnout % |
| 🔽 **Year Slicer** | Filters all visuals to a selected election year |

**Purpose:**
To identify long-term patterns, participation changes, and shifts in party performance across elections.

---

### 3️⃣ Real-Time Results

This dashboard simulates a live election night reporting interface, dynamically updating based on the selected year.

**Key Visuals:**

| Visual | Description |
|---|---|
| 🃏 **KPI Card** | Leading Party — party with the most seats won for the selected year |
| 🃏 **KPI Card** | Seats Won — total seats secured by the leading party |
| 🃏 **KPI Card** | Majority Mark — seat threshold required to form a majority government |
| 🃏 **KPI Card** | Total Votes — aggregate votes cast in the selected year |
| 📈 **Column Chart** | Seat Distribution by Party — bar chart of seats won per party |
| 🥧 **Pie Chart** | Seat Share Distribution — proportional seat share across all parties |
| 📋 **Winners Table** | Constituency, Candidate, Votes, and Party for all winning candidates |
| 🔽 **Year Slicer** | Filters all visuals to display results for the chosen election year |

**Purpose:**
To provide a real-time style summary of election outcomes — who won, by how much, and where — for a selected year.

---

### 4️⃣ Voter Turnout & Demographic Insights

This dashboard focuses on voter participation patterns across constituencies and election years.

**Key Visuals:**

| Visual | Description |
|---|---|
| 🃏 **KPI Card** | Highest Participation % — constituency with the highest voter turnout |
| 🃏 **KPI Card** | Average Voter Turnout — mean turnout percentage across all constituencies |
| 🃏 **KPI Card** | Lowest Participation % — constituency with the lowest voter turnout |
| 📉 **Line Chart** | Voter Participation Trend Across Elections — tracks average turnout by year |
| 📊 **Bar Chart** | Top 10 Constituencies by Voter Turnout — ranks the most engaged constituencies |
| 🍩 **Donut Chart** | Turnout Category distribution — groups constituencies by turnout range |
| 🌳 **Treemap** | Constituency-wise vote volume — sized by total votes cast |
| ⏲️ **Gauge** | Voter Engagement Level — overall engagement score metric |
| 🔽 **Year Slicer** | Filters all visuals to a selected election year |

**Purpose:**
To highlight areas with strong civic engagement and identify regions with lower participation, helping understand demographic voting patterns.

---

### 5️⃣ Party & Candidate Insights

This dashboard analyzes individual party and candidate performance across elections.

**Key Visuals:**

| Visual | Description |
|---|---|
| 🃏 **KPI Card** | Top Candidate — candidate with the highest individual vote count |
| 🃏 **KPI Card** | Leading Party — party with the most seats won |
| 🍩 **Donut Chart** | Party-wise seat share — proportion of seats won by each party |
| 📊 **Bar Chart** | Number of Candidates vs. Votes — compares candidate count to total votes by party |
| ⚡ **Scatter Chart** | Candidate-level scatter — plots total votes vs. turnout % per candidate |
| 🌳 **Treemap** | Party vote volume — sized by total votes received per party |
| 📈 **Column Chart** | Number of Candidates by Party — shows how many candidates each party fielded |
| 🔽 **Year Slicer** | Filters all visuals to a selected election year |

**Purpose:**
To analyze the dominance of political parties and performance of individual candidates, revealing vote distribution and competitive dynamics.

---

## 🧮 Key DAX Measures

| Measure | Description |
|---|---|
| **Seats Won** | Count of constituencies won per party |
| **Leading Party** | Dynamic measure returning the party with the most seats won |
| **Majority Mark** | Calculated threshold for a majority (total constituencies / 2 + 1) |
| **Constituency Vote Growth %** | Year-over-year vote growth percentage per constituency |
| **Average Voter Turnout** | Mean turnout % across all constituencies |
| **Highest / Lowest Participation %** | Max and min turnout values across constituencies |
| **Engagement Score** | Composite metric representing overall voter engagement level |
| **Total Constituencies** | Count of distinct constituencies in the dataset |
| **Total Parties** | Count of distinct parties in the dataset |
| **Top Candidate** | Candidate with the highest individual vote total |

---

## 🛠 Tools & Technologies Used

- **Microsoft Power BI Desktop** — report authoring and dashboard design
- **DAX (Data Analysis Expressions)** — custom measures and calculated columns
- **Power Query (M Language)** — data transformation and loading
- **Data Modeling** — relationships between election year tables
- **Git & GitHub** — version control and project hosting

---

## 📂 Repository Structure

```
ElectViz-Election-Data-Visualization/
├── ElectViz.pbix       # Power BI report file (open with Power BI Desktop)
├── Script.txt          # Supporting scripts
└── README.md           # Project documentation
```

## 🚀 Getting Started

1. Download and install [Microsoft Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free for personal use).
2. Clone or download this repository.
3. Open `ElectViz.pbix` in Power BI Desktop.
4. Use the **Year Slicer** on each dashboard page to filter results by election year (2009, 2014, 2019).
5. Navigate between the 5 dashboard pages using the tabs at the bottom of the report.
