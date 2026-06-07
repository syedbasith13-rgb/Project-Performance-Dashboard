# Project Performance Dashboard

## Overview

This project presents an interactive Power BI dashboard designed to monitor project performance across multiple AI initiatives. The dashboard provides operational leaders with a centralized view of productivity, quality, rework, workload distribution, and project health to support data-driven decision-making.

---

## Business Objective

The objective of this dashboard is to:

* Monitor project and associate performance.
* Track quality and rework trends.
* Identify operational risks and coaching opportunities.
* Compare project performance across key operational metrics.
* Support continuous improvement through actionable insights.

---

## Dataset

A synthetic AI operations dataset was created to simulate the performance of a team consisting of AI Tutors, Verifiers, and Super Verifiers working across multiple AI projects.

### Dataset Highlights

* 25 Associates
* 5 Active Projects
* Multiple Roles
* Daily Performance Records
* Quality Scores
* Rework Metrics
* Hours Worked
* Tasks Completed
* SLA Metrics

### Projects Included

* Atlas
* Nova
* Orion
* Titan
* Helios

---

## Data Model

The dashboard follows a Star Schema design.

### Fact Table

**Fact_Performance**

Contains operational performance records including:

* Date
* Employee ID
* Project ID
* Tasks Completed
* Hours Worked
* Quality Score
* Rework Tasks
* SLA %

### Dimension Tables

**Dim_Employee**

* Employee ID
* Employee Name
* Role

**Dim_Project**

* Project ID
* Project Name

**Date Table**

* Calendar Date

### Relationships

* Fact_Performance → Dim_Employee (Many-to-One)
* Fact_Performance → Dim_Project (Many-to-One)
* Fact_Performance → Date Table (Many-to-One)

Single-direction filtering was implemented to maintain a clean and efficient star schema model.

---

## Dashboard Pages

### Executive Overview

Provides a high-level summary of operational performance.

#### KPIs

* Total Employees
* Total Active Projects
* Total Tasks Completed
* Average Quality Score
* Average SLA %

#### Analysis

* Tasks Completed by Project
* Quality Score by Project
* Hours Worked by Project
* Productivity by Project
* Rework Tasks by Project

---

### Associate Performance Analysis

Provides detailed analysis of individual associate performance.

#### KPIs

* Team Productivity
* Highest Quality Score
* Lowest Rework %
* Highest Productivity

#### Analysis

* Quality vs Rework Scatter Plot
* Associate Performance Matrix
* Project-Based Filtering
* Role-Based Filtering

#### Key Findings

* Neha achieved the highest quality score while maintaining the lowest rework rate.
* Rohan recorded the highest rework rate and lowest quality score, indicating a coaching opportunity.
* Imran and Isha require monitoring due to elevated rework rates and lower quality performance.
* Sara worked on fewer projects than her peers, highlighting an opportunity for cross-training.

---

### Project Health Analysis

Evaluates project performance and operational risk.

#### Analysis

* Project Quality vs Rework Analysis
* Project Performance Matrix
* Productivity Comparison
* Workload Comparison

#### Key Findings

* Project Nova recorded the lowest quality score and highest rework rate, making it the highest-risk project.
* Project Titan demonstrated the strongest overall performance with the highest productivity and strong quality metrics.
* Project Helios maintained stable and consistent performance across key KPIs.
* Atlas and Orion performed within acceptable limits but should continue to be monitored.

#### Recommendations

* Conduct a Root Cause Analysis (RCA) on Project Nova to identify factors impacting quality and rework.
* Review workflows and best practices implemented within Titan and Helios.
* Monitor Atlas and Orion and implement targeted improvement initiatives where required.

---

## Skills Demonstrated

* Power BI
* Power Query
* DAX
* Data Modeling
* Star Schema Design
* KPI Development
* Data Visualization
* Dashboard Storytelling
* Business Intelligence
* Performance Analytics

---

## Files Included

* Project Performance Dashboard.pbix
* Dashboard Screenshots
* README.md

---

## Author

**Syed A. Basith**
