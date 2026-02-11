# Insurance Data Analysis – Power BI Dashboard

## Project Summary
This project delivers an end-to-end insurance analytics solution using SQL and Power BI to analyze policy performance, claims behavior, and customer sentiment for decision-making.

The dashboard helps stakeholders understand:
- Premium revenue performance
- Claim distribution and claim status trends
- Policy activity trends
- Customer segmentation by age group and policy type
- Customer feedback sentiment and common service issues

### Business Objectives
This dashboard addresses key business questions such as:
- Which **Policy Types** generate the most premium?
- What are the **claim approval vs rejection** patterns?
- How do **claims vary by age group**?
- What is the relationship between **Premium vs Claim Amount**?
- What are the key **customer satisfaction trends** from feedback?

Designed and delivered an enterprise-style Power BI reporting solution with **Row-Level Security (RLS)** and KPI monitoring.

### Dataset Overview
- **Total Policies:** 10,000  
- **Total Customers:** 10,000  
- **Total Claims:** 5,646  
- **Data Time Range:** July 2023 – July 2025  

## Dataset Fields:
- Policy Number
- Customer ID
- Policy Type
- Claim Status
- Coverage Amount
- Premium Amount
- Claim Amount
- Policy Start Date / Policy End Date
- Age Group
- Customer Feedback

### Data Modeling
- Built a **report-ready model** to support filtering by Policy Type, Claim Status, and Age Group
- Created DAX measures for KPI reporting and segmentation analysis
- Ensured efficient filter behavior and clean report performanceperformance.

### Tools & Technologies
- SQL (data exploration / querying)
- Power BI Desktop
- Power Query (ETL)
- DAX
- Power BI Service (Publishing, RLS, Scheduled Refresh)

### Technical Highlights
- Built dynamic KPI cards using DAX (Premium Amount, Coverage Amount, Claim Amount)
- Implemented drill-through and cross-filtering for deeper analysis
- Cleaned and transformed data using Power Query (ETL)
- Implemented **Row-Level Security (RLS)** for role-based access
- Performed sentiment analysis using Power BI AI features to classify customer feedback
- Developed optimized DAX measures using `CALCULATE`, `FILTER`, and aggregations
- Implemented dynamic date filtering for policy lifecycle analysis


### Row-Level Security (RLS) Implementation
Implemented role-based access control to restrict managers to their respective **Policy Types**.

Steps:
1. Created roles in Power BI Desktop with PolicyType filters
2. Tested using **View as Role**  
3. Published to Power BI Service
4. Assigned users to roles and validated permissions in Power BI Service  

## How to Use the Dashboard
- Use slicers (PolicyType, ClaimStatus, AgeGroup) to filter insights
- Use drill-through to investigate policy and claim details by segment
- Review Customer Feedback page to track sentiment categories and commonly reported service issues.

## Dashboard Snapshots (Power BI)
### Executive Overview Dashboard
![Executive Overview](images/executive_overview_dashboard.png)

**Highlights:**
- KPI cards (Premium Amount, Coverage Amount, Claim Amount)
- Premium by Policy Type
- Claim Status distribution
- Claim Amount by Age Group
- Active vs Inactive policies

### Policy & Claims Details
![Policy & Claims](images/policy_claims_analysis.png)

**Highlights**
- Policy-level drill-through
- Policy start/end timeline analysis
- Claim history by policy type and status

### Customer Feedback & Sentiment
![Customer Feedback](images/customer_feedback_dashboard.png)

**Highlights**
- Sentiment classification (e.g., Positive/Neutral/Negative or category-based)
- Most common terms from feedback
- Frequent issues: response delays and documentation clarity

### Key Insights
- **Total Premium Amount:** 5.97M  
- **Total Coverage Amount:** 600.33M  
- **Total Claim Amount:** 16.90M
- Claims-to-premium comparison indicates potential margin pressure in high-coverage segments
- Travel policies generated the highest premium revenue
- ~58% of policies are Active, indicating strong portfolio engagement
- Rejected claims are higher than pending claims, suggesting documentation/underwriting gaps
- Adult age group shows the highest claim amounts, indicating higher risk exposure in this segment

## Data Ethics & Disclaimer
This project uses a synthetic/anonymized dataset for learning and portfolio purposes.
It does not represent real customer or insurance data.
