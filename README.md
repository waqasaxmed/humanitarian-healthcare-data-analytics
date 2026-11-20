# Assessing Primary Healthcare Facility Performance and Resource Allocation in Humanitarian Settings

**Capstone Data Analytics Project | Synthetic Data**

## Project Overview

This project explores primary healthcare facility performance, operational constraints, and resource allocation using a synthetic dataset representing 40 primary healthcare centres (PHCCs) across three governorate groupings over a 24-month period.

The project applies a structured data analytics workflow to examine service utilisation patterns, explore relationships between operational indicators and healthcare utilisation, assess resource allocation, and identify facilities requiring further management investigation.

The project demonstrates how data analytics can transform multiple datasets into actionable insights to support monitoring, resource allocation review, and evidence-informed decision-making in humanitarian healthcare settings.

> \*\*Disclaimer:\*\* All datasets and findings in this project are synthetic and illustrative. They do not represent actual healthcare facilities, humanitarian programmes, or operational findings.

---

## Problem Statement

Healthcare programme monitoring often involves multiple datasets containing service utilisation, facility functionality, staffing, supply availability, and financial information.

Reviewing these indicators individually may limit the ability to identify patterns, understand operational concerns, and assess whether resource allocation reflects facility demand and constraints.

This project explores how integrating these indicators into a structured analytical framework can provide a more comprehensive perspective on healthcare facility performance and support management decision-making.

---

## Analytical Objectives

The analysis aimed to:

- Examine service utilisation patterns across facilities and over time.
- Explore associations between operational constraints and service utilisation.
- Assess the distribution of financial resources across facilities.
- Examine relationships between resource allocation, demand, and operational constraints.
- Develop a rule-based screening framework to identify facilities requiring further investigation.

---

## Dataset

The project uses a synthetic dataset covering:

| Dataset characteristic | Description |
|---|---|
| Healthcare facilities | 40 PHCCs |
| Geographical groupings | Raqqa, Hasakeh, and Aleppo |
| Time period | January 2024 – December 2025 |
| Observation frequency | Monthly |
| Facility-month records | 960 |
| Variables in integrated dataset | 40 |

### Datasets

- `PHCC\_Master.csv` — Facility characteristics and geographical information
- `PHCC\_Monthly\_Performance.csv` — Monthly service utilisation and operational indicators
- `PHCC\_Monthly\_Resources.csv` — Monthly resource allocation and expenditure information
- `PHCC\_Integrated\_Analytical\_Dataset.csv` — Consolidated analytical dataset

---

## Analytical Workflow

The project followed a structured analytical workflow:

### 1. Data Preparation and Cleaning

- Dataset structure and variable review
- Missing-value assessment
- Duplicate identification and removal
- Data validation and anomaly assessment
- Dataset integration
- Verification of calculated indicators
- Financial reconciliation checks

### 2. Exploratory Data Analysis (EDA)

- Descriptive statistics
- Monthly service utilisation trends
- Facility-level comparisons
- Distribution analysis
- Operational indicator assessment
- Financial allocation and expenditure analysis

### 3. Statistical Analysis

Statistical methods were used to explore relationships and differences within the dataset, including:

- Pearson correlation
- Spearman rank correlation
- Kruskal–Wallis test

The statistical findings were interpreted alongside descriptive analysis and contextual limitations.

### 4. Management Prioritisation

A rule-based screening framework was developed using four operational warning indicators:

- Staffing constraints
- Stock-out concerns
- Reduced facility functionality
- Low service utilisation

Facilities were categorised according to the number of warning flags identified to support management review and follow-up.

### 5. Dashboard Development

An interactive Power BI dashboard was developed to present the principal findings and enable exploration of facility-level information.

---

## Key Findings

### 1. Service Utilisation Varied Across Facilities and Over Time

Monthly consultations ranged from approximately **334,389 to 540,854**, with noticeable fluctuations and periods of decline and subsequent recovery.

Facility-level utilisation also varied considerably, highlighting the importance of examining both temporal trends and differences between facilities.

### 2. Facility Functionality Demonstrated a Stronger Association with Utilisation

Consultation rates differed across facility functionality categories:

| Functionality status | Mean consultations per service day |
|---|---:|
| Fully functional | 525.86 |
| Partially functional | 396.34 |
| Temporarily disrupted | 235.65 |

The differences between functionality groups were statistically significant using the Kruskal–Wallis test.

### 3. Stock-outs Were Weakly Associated with Lower Utilisation

Stock-out days demonstrated a weak negative association with consultations per service day, while staffing availability showed no meaningful association within this dataset.

### 4. Resource Allocation Was Strongly Associated with Service Utilisation

Facilities with higher consultation volumes generally received higher resource allocations. However, allocation did not demonstrate clear relationships with several operational constraint indicators, including staffing availability, stock-out levels, and facility functionality.

### 5. Analytical Prioritisation Identified Facilities for Further Investigation

The rule-based screening framework identified:

- **4 high-priority facilities**
- **10 moderate-priority facilities**
- **14 facilities in total requiring further investigation**

The framework demonstrates how multiple operational indicators can be combined to support structured management review.

These categories represent analytical screening priorities, not definitive facility performance rankings.

---

## Power BI Dashboard

The dashboard consists of three interactive pages.

### Page 1 — Overall PHCC Performance

Explores service utilisation, monthly trends, and facility-level comparisons across key operational indicators.

### Page 2 — Resource Allocation

Examines resource distribution, expenditure, budget utilisation, and relationships between allocation and service utilisation.

### Page 3 — Management Prioritisation

Highlights facilities requiring further investigation using a rule-based operational screening framework.

---

## Tools and Technologies

- **Python** — Data preparation, cleaning, analysis, and statistical exploration
- **Power BI** — Interactive dashboard development and data visualisation
- **Statistical analysis** — Correlation analysis and non-parametric testing
- **Data analytics** — Data validation, exploratory analysis, interpretation, and management-oriented insights

---

## Limitations

- The dataset is entirely synthetic and does not represent real-world operational evidence.
- Consultation volumes do not independently measure healthcare quality, effectiveness, or unmet need.
- Observations are repeated monthly for the same facilities, limiting the independence assumption of some statistical tests.
- Correlation does not establish causation.
- Management prioritisation thresholds are illustrative and have not been externally validated.

---

## Project Structure

```text

Capstone\_1/

│

├── README.md

│

├── Data/

│   ├── PHCC\_Master.csv

│   ├── PHCC\_Monthly\_Performance.csv

│   ├── PHCC\_Monthly\_Resources.csv

│   └── PHCC\_Integrated\_Analytical\_Dataset.csv

│

├── Python/

│   └── Capstone\_Analysis.ipynb

│

├── PowerBI/

│   └── Capstone1\_PHCC\_Performance\_Resource\_Allocation.pbix

│

├── Report/

│   └── Capstone1\_Analytical\_Report.docx

│

└── Screenshots/

&#x20;   ├── Page1\_Performance.png

&#x20;   ├── Page2\_Resource\_Allocation.png

&#x20;   └── Page3\_Management\_Prioritisation.png

```

---

## Project Outcome

This capstone demonstrates an end-to-end data analytics workflow—from dataset preparation and validation through exploratory and statistical analysis, interpretation of findings, management prioritisation, and interactive dashboard development.

The project emphasises not only analytical techniques, but also the ability to translate data into meaningful insights and practical management questions.

**Key skills demonstrated:** Data cleaning, data integration, exploratory data analysis, statistical interpretation, correlation analysis, non-parametric testing, data visualisation, dashboard development, and analytical storytelling.
