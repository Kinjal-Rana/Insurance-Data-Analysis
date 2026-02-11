# Insurance Data Analysis – Power BI Dashboard

## Project Summary
This project delivers an end-to-end insurance analytics solution using SQL and Power BI to analyze policy performance, claims behavior, and customer sentiment for strategic decision-making.

The dashboard helps stakeholders understand:
- Premium revenue performance
- Claim distribution and status
- Policy activity trends
- Customer segmentation
- Customer sentiment insights

### Business Objectives
This dashboard addresses critical business questions such as:
- Policy performance by type
- Claim approval and rejection patterns
- Active vs inactive customers
- Revenue (Premium) vs Claim payouts
- Customer satisfaction trends

Delivered an enterprise-style Power BI reporting solution enabling secure, role-based access and strategic performance monitoring.

### Dataset Overview
- Total Policies: 10,000
- Total Customers: 10,000
- Total Claims: 5646
- Data Time Range: July 2023–July 2025
- Dataset Features:
	- Policy Number
	- Customer ID
	- Policy Type
	- Claim Status
	- Coverage Amount
	- Premium Amount
	- Claim Amount
	- Age Group
	- Customer Feedback

### Data Model
- Designed star schema model
- Created relationships between Policy, Claims, and Customer tables
- Implemented calculated columns and DAX measures

### Tools & Technologies
- MySQL Server – Data storage
- SQL – Data querying
- Power BI Desktop
- Power Query
- DAX
- Power BI Service (Publishing + RLS + Scheduled Refresh)

### Technical Highlights
- Built dynamic KPI cards using DAX
- Implemented drill-through and cross-filtering
- Performed data cleansing and transformation using Power Query (ETL process).
- Implemented Row-Level Security (RLS) for secure, role-based data access.
- Implemented customer sentiment analysis using Power BI AI Text Analytics.

### Row-Level Security (RLS) Implementation
To ensure data confidentiality, Row-Level Security (RLS) was implemented so that each manager can view only the specific Policy Type relevant to them.

Implemented role-based access control to restrict managers to their respective Policy Types. Roles were created and tested in Power BI Desktop and validated in Power BI Service.

## Dashboard Snapshots (Power BI)
### Insurance Dashboard Overview
![Insurance Dashboard](images/executive_overview_dashboard.png)

Main Insurance Dashboard Overview
**Highlights:**
- KPI cards (Premium, Coverage, Claim Amount)
- PolicyType revenue breakdown
- Claim Status distribution
- Claim Amount by Age Group
- Active vs Inactive policies

### Policy & Claims Analysis
![Policy & Claims Analysis](images/policy_claims_analysis.png)

Features:
- Drill-through functionality by PolicyType
- Non-aggregated fields
- Policy Start/End tracking
- Claim history tracking

### Customer Feedback Analysis
![Customer Feedback Analysis](images/customer_feedback_dashboard.png)

Implemented:
- Power BI AI Text Analytics
- Sentiment scoring (0 to 1 scale)
- Categorized feedback:
	- Excellent
	- Good
	- Needs Improvement

Insight:
- Sentiment scoring indicates predominantly positive customer feedback.
- Common issues: response delay & policy documentation clarity

### Key Insights
- Total Premium Revenue: 5.97M
- Total Coverage Value: 600.33M
- Total Claims Paid: 16.90M
- Claims-to-premium analysis indicates margin pressure in high-coverage policy segments.
- Travel policies generated the highest premium revenue.
- 58% of policies are Active, indicating strong portfolio engagement.
- Rejected claims exceed pending claims, indicating potential underwriting or documentation gaps.
- Adult age group accounts for the highest claim amounts, indicating higher risk exposure in this segment.
