📉 Customer Churn Analysis Dashboard — Power BI

Built during Saiket Systems Remote Internship (March 2026)
An end-to-end customer churn analysis dashboard using the IBM Telco dataset, featuring KPI tracking, churn segmentation, revenue risk analysis, and DAX-powered metrics.


📌 Project Overview
ItemDetailsDatasetIBM Telco Customer ChurnToolPower BI DesktopSkillsDAX · Power Query · Data Modeling · ETLOutputInteractive .pbix DashboardOrganizationSaiket Systems (Remote Internship)

📊 Dashboard KPIs
KPIDescriptionChurn Rate %% of customers who leftRevenue at RiskMonthly revenue from churned customersContract Type BreakdownMonth-to-month vs 1yr vs 2yrRetention SegmentsHigh / Medium / Low churn risk groupsTenure DistributionChurn by customer tenureInternet Service AnalysisFiber vs DSL vs No service churn rates

🔧 Technical Implementation
Data Cleaning (Power Query)

Removed blanks and null values
Converted TotalCharges from text to numeric
Created Churn Flag binary column (1/0)

DAX Measures
Churn Rate = DIVIDE([Churned Customers], [Total Customers])
Revenue at Risk = SUMX(FILTER(Customers, Customers[Churn]="Yes"), Customers[MonthlyCharges])
Avg Tenure (Churned) = CALCULATE(AVERAGE(Customers[tenure]), Customers[Churn]="Yes")
Data Model

Star schema with Customers as fact table
Relationships: Contract · PaymentMethod · InternetService


📁 Files
FileDescriptionsaiket.pbixPower BI Dashboard fileREADME.mdProject documentation

💡 Key Insights

Month-to-month contract customers churn 3x more than annual contract customers
Fiber optic customers have the highest churn rate despite being a premium product
Customers with tenure < 12 months account for majority of churn
Electronic check payment method correlates with highest churn


🛠️ Tools Used
Power BI Desktop · DAX · Power Query · Data Modeling · ETL · IBM Telco Dataset

👤 Author
Kashish Yadav — Data Analyst Intern @ Saiket Systems

📧 kashishrao68@gmail.com
💼 LinkedIn
🐙 GitHub
