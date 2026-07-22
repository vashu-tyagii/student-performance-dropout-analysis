# EdTech Student Performance & Dropout Analysis

## Objective
Analyze student academic and demographic data to identify patterns behind
low attendance, low scores, and dropout risk.

## Dataset
Source: Kaggle — search for one of these (free, public):
- "Students Performance in Exams" (spscientist)
- "Student Alcohol Consumption" (uciml)
- "Predict Students Dropout and Academic Success" (UCI ML Repository)

Download the CSV and place it in `data/raw/`.

## Folder Structure
```
project1-edtech/
├── data/
│   ├── raw/              -> original downloaded CSV (never edit this)
│   └── cleaned/          -> output after cleaning script
├── sql/
│   └── queries.sql       -> SQL you ran (table creation + analysis queries)
├── notebooks/
│   └── analysis.ipynb    -> Python/Pandas cleaning + EDA
├── dashboard/
│   └── edtech_dashboard.pbix   -> Power BI file
│   └── dashboard_screenshot.png
└── README.md             -> this file, update with REAL findings at the end
```

## Steps To Actually Do This
1. Load CSV into a SQL table (SQLite is fine, or MS SQL Server if installed).
2. Write SQL queries: average score by gender, by parental education,
   by test-prep-course completion.
3. In Python (Pandas): clean nulls, check data types, compute correlations
   (e.g. attendance vs. score, if the dataset has attendance data).
4. Bring cleaned data into Power BI. Build 3-4 visuals:
   - Score distribution by category
   - A correlation/scatter visual
   - A KPI card for an overall average
5. **Write down the REAL number you find** — whatever it is, even if it's
   small or unexciting. That number goes in your resume, not before.

## What To Put In Resume (only after this is done)
Replace the placeholder bullet with your actual finding, e.g.:
"Found that students who completed the test preparation course scored
on average X points higher than those who didn't."
(X = whatever your data actually shows — could be 5, could be 15. Use the real one.)
