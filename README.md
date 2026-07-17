# Smartphone Market Analytics

Applied Learning Project, MBA Semester 3 (Data Science & Analytics), Jain Online.

## What this is

A retailer ("Saap" in the case brief) wants to know what actually drives smartphone pricing, adoption, and customer satisfaction: device specs, or who's buying. This project answers that with a two-stage analysis: statistical testing in Python, then an interactive Tableau workbook built on the same findings.

The underlying dataset (990 records, 22 variables: device specs plus buyer demographics) was provided as part of the coursework and isn't included in this repo, since it isn't mine to redistribute. The notebook and Tableau workbook both expect a cellphone_data.csv in data/ with the same schema if you want to rerun the analysis.

## Key findings

Finding 1: Brand, not specs, drives price. ANOVA across brands: F = 105.69, p < 0.001.

Finding 2: OS defines the hardware tier. iOS and Android split cleanly on RAM (F = 143.92) and screen size (F = 389.85); brand and OS are effectively the same variable (chi-square, approx 990, p < 0.001).

Finding 3: Demographics don't predict device choice. Age, gender, and occupation showed no significant effect on price category, brand, or OS preference. Broad demographic targeting doesn't hold up here; specification-based targeting does.

Finding 4: Regional income gaps show up in the data. Mumbai salaries came in significantly higher than Delhi's (p = 0.00024), and that maps to premium-tier representation by city.

Full test log (18 hypothesis tests: t-tests, ANOVA, chi-square) is in the notebook and summarized in the report.

## Repo structure

notebooks/ holds the Python analysis: cleaning, EDA, hypothesis testing (Pandas, SciPy, Seaborn).
tableau/ holds the .twbx workbook: 2 dashboards, 15 worksheets, 12-point storyboard.
report/ holds the full write-up: methodology, findings, business recommendations.

## Tools

Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy), Jupyter, Tableau Desktop.

## Reproducing the analysis

Supply your own cellphone_data.csv in data/ (see "What this is" above), then run pip install -r requirements.txt and jupyter notebook notebooks/.

Open tableau/smartphone_market_analytics.twbx in Tableau Desktop (or Tableau Public) for the dashboards and storyboard.

## Status

Coursework project, submitted for MBA Semester 3. Not maintained as production code; treat it as a snapshot of the analysis, not a live tool.
