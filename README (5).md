# IncidentIQ: IT Incident Management Analysis using Python

## Project Overview
IncidentIQ analyses 141,712 historical IT incident records to evaluate incident
management performance, SLA compliance, workload distribution and ticket trends.
Using Python, it covers data cleaning, feature engineering, exploratory data
analysis (EDA) and business recommendations.

## Problem Statement
IT Service Management (ITSM) teams handle thousands of incidents. Without analysis
it is hard to monitor SLA compliance, spot recurring issues, balance workloads,
and find bottlenecks. This project answers those questions from historical data.

## Dataset
- **Name:** Incident Management Process Enriched Event Log (UCI Machine Learning Repository)
- **Size:** 141,712 records, 36 columns
- **Fields include:** incident number, state, priority, impact, urgency, assignment group,
  category, contact type, opened/resolved/closed dates, SLA status, reassignment and reopen counts

See `dataset/README.md` for download steps.

## Tools
Python, Pandas, NumPy, Matplotlib, Jupyter Notebook

## EDA Covered
Status distribution, SLA compliance, priority / impact / urgency, priority vs SLA,
assignment group workload, top categories and subcategories, contact channel,
monthly / daily / hourly trends, resolution time, top resolvers, correlation of operational metrics.

## Key Findings
- About 93.5% of incidents met the defined SLA.
- Most incidents were Moderate priority and Medium impact, so routine issues dominate the workload.
- Volume was concentrated in a small number of categories and assignment groups.
- Ticket creation followed clear hourly, daily and monthly patterns.
- Workload was unevenly spread across assignment groups and engineers.

## Recommendations
- Improve ticket routing to reduce reassignments.
- Track SLA compliance on a live dashboard.
- Write knowledge-base articles for recurring incidents.
- Staff according to peak periods.
- Investigate long-resolution incidents.
- Improve assignment group data quality.

## Repository Structure
```
incidentiq-it-incident-analysis/
├── IncidentIQ.ipynb
├── README.md
├── requirements.txt
├── LICENSE
├── .gitignore
├── dataset/
│   └── README.md        (put incident_event_log.csv here)
└── images/
    └── (exported charts)
```

## Getting Started
```bash
git clone https://github.com/rohinidatkar/incidentiq-it-incident-analysis.git
cd incidentiq-it-incident-analysis
pip install -r requirements.txt
# download the dataset into dataset/ (see dataset/README.md)
jupyter notebook
```
Open `IncidentIQ.ipynb` and run all cells.

## Saving charts
Add this after any plot in the notebook, then commit the files in `images/`:
```python
plt.savefig("images/sla_compliance.png", dpi=150, bbox_inches="tight")
```

## Future Enhancements
SLA breach prediction, priority prediction, volume forecasting, anomaly detection,
Power BI dashboard, SQL-based analytics, Streamlit dashboard.

## Skills Demonstrated
Data cleaning, feature engineering, EDA, data visualisation, KPI reporting,
incident management analytics, root cause analysis, Python.

## Contact
Rohini Datkar, Pune, Maharashtra | rohinidatkar@gmail.com
[LinkedIn](https://www.linkedin.com/in/rohinidatkar/) | [GitHub](https://github.com/rohinidatkar)
