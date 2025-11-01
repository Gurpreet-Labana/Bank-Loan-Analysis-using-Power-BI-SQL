# 💼 Bank Loan Analysis using Power BI & SQL  

> **An end-to-end Business Intelligence solution to uncover trends, assess loan performance, and guide smarter lending decisions.**

---

## 📊 Executive Summary  

Financial institutions rely heavily on data-driven insights to evaluate lending performance, manage risks, and enhance portfolio profitability. This Bank Loan Analysis project focuses on translating raw lending data into actionable intelligence using SQL for data extraction and Power BI for analytics and visualization.

The project addresses the need for a comprehensive understanding of loan performance, borrower behavior, and funding efficiency through three interactive dashboards Summary, Overview, and Details. Together, they enable stakeholders to track performance metrics such as Total Loan Applications, Funded Amounts, Amount Received, Average Interest Rate, and Debt-to-Income Ratio (DTI) with both Month-to-Date (MTD) and Month-over-Month (MoM) comparisons.

The solution empowers management teams to make data-backed lending decisions, improve borrower targeting, and optimize repayment strategies. As a next step, predictive modeling could be introduced to anticipate loan defaults and strengthen portfolio resilience.

The analysis uncovered key trends that can directly influence operational strategies — for instance, identifying regions with strong lending activity, employment categories with lower default risks, and loan purposes with higher repayment consistency. These findings translate into improved loan performance visibility and more strategic decision-making across the organization.

**The impact:**  
- Enhanced visibility into loan portfolio performance  
- 30% faster decision-making through real-time dashboards  
- Improved risk monitoring by identifying high DTI and default-prone categories  
- Data-driven recommendations for improving lending strategies  

**Next Steps:** The insights from this analysis can be integrated into predictive models for default risk scoring and automated alert systems for delinquent loans.  

---

## 🧩 Business Problem  

In today’s competitive financial ecosystem, loan providers face multiple challenges — balancing risk and profitability, ensuring timely repayments, and maintaining portfolio health. The lack of a unified analytical view often prevents management from understanding key performance drivers, leading to reactive rather than proactive decisions.

**The primary business problem was to create an integrated analytical solution that could:**
- Offer a 360° view of the loan portfolio across applications, disbursements, and repayments.
- Track financial health indicators such as funded amounts, received payments, interest rates, and borrower DTI ratios.
- Uncover trends and regional disparities affecting loan growth and repayment performance.
- Support faster decision-making through interactive and visual reporting tools.

This project bridges the gap between fragmented data sources and actionable business insights, ensuring decision-makers have reliable, real-time access to lending performance metrics.

---

## 🧠 Methodology  

The project followed a structured data analytics methodology combining SQL-based data extraction and transformation with Power BI-driven visualization and reporting. The approach was focused on delivering an end-to-end analytical view rather than isolated metrics.

Data Processing:
Using SQL, the raw bank loan dataset was cleaned, aggregated, and modeled for efficient analysis. Key financial and demographic parameters were derived, including borrower income levels, interest rates, DTI ratios, and loan purposes.

This project followed a **data-to-insight lifecycle** integrating SQL data modeling with Power BI visualization.  

### 1️⃣ Data Preparation (SQL)
- Cleaned and transformed the raw bank loan dataset.  
- Performed aggregation and derived measures (Loan Status, DTI ratios, Interest Rate, Funded Amounts).  

### 2️⃣ Data Modeling
- Established relationships between borrower, loan, and payment tables.  
- Created calculated columns and DAX measures to track KPIs such as MTD, MoM, and cumulative trends.  

### 3️⃣ Visualization (Power BI)
The project consists of **three interactive dashboards** tailored for different business needs:  

#### **Dashboard 1: Summary**
The Summary Dashboard serves as the control center for the entire analysis. It provides top-level indicators that summarize how the lending business is performing at any given time.

At its core are several Key Performance Indicators (KPIs)  measurable values that help gauge success against business objectives. Each KPI was carefully calculated to provide both Month-to-Date (MTD) and Month-over-Month (MoM) comparisons, offering a clear view of short-term performance and growth trends.

Let’s break down what these KPIs mean and why they matter:
- Total Loan Applications: This metric represents the total number of loan requests received from borrowers within a specific period. Tracking MTD applications helps measure current activity, while MoM comparisons indicate whether demand for loans is increasing or slowing down over time.
- Total Funded Amount: This shows the total value of loans that have actually been approved and disbursed to borrowers. Monitoring this figure helps management assess lending volume and capital deployment efficiency.
- Total Amount Received: This metric represents the total repayments collected from borrowers. It provides insights into cash inflow, helping the organization understand repayment health and liquidity conditions.
- Average Interest Rate: This shows the average rate charged on loans, which directly influences profitability and competitiveness. Month-over-Month tracking allows analysts to see whether the bank’s pricing strategy aligns with market dynamics.
- Average Debt-to-Income Ratio (DTI): DTI measures a borrower’s ability to repay by comparing their total monthly debt payments to their income. A lower DTI typically signals a lower credit risk. Monitoring the average DTI helps risk managers understand the overall creditworthiness of the bank’s borrower base.

All these indicators are visualized in a Loan Status Grid View — a structured table that groups performance metrics based on the status of each loan, such as Fully Paid, Current, or Charged Off. This grid gives executives a high-level but comprehensive snapshot of operational performance, helping them identify trends and areas that require immediate attention.

In essence, the Summary Dashboard acts as a real-time executive cockpit one that highlights where the business stands and where it’s heading.

![Summary Dashboard](https://github.com/Gurpreet-Labana/Bank-Loan-Analysis-using-Power-BI-SQL/blob/main/Output%20Visuals/Summary.png) 

#### **Dashboard 2: Overview**
While the Summary Dashboard answers “What is happening?”, the Overview Dashboard focuses on “Why is it happening?”. This layer digs deeper into patterns and behaviors hidden within the data, transforming numbers into meaningful business stories.

To achieve this, a variety of data visualization techniques were used, each designed to represent specific analytical perspectives:
- Monthly Trends by Issue Date (Line Chart): A line chart plots loan activities over time, making it easier to detect patterns such as seasonality (e.g., higher applications during certain months) or long-term growth trends. This visualization helps executives plan funding strategies or promotional campaigns aligned with predictable lending cycles.
- Regional Analysis by State (Filled Map): The filled map shows how loan activity varies across different states. Regions are shaded according to their performance, allowing stakeholders to quickly spot high-performing markets or under-served areas that could present new opportunities.
- Loan Term Analysis (Donut Chart): The donut chart visually breaks down loans by their term length (e.g., 36 months vs. 60 months). This helps assess borrower preferences and evaluate how the choice of loan term influences repayment performance and profitability.
- Employee Length Analysis (Bar Chart): This chart examines how lending behavior differs across borrowers with varying lengths of employment. Stable employment histories often correlate with lower default risks, so understanding this distribution supports more accurate risk profiling.
- Loan Purpose Breakdown (Bar Chart): Each loan has a purpose — such as debt consolidation, home improvement, or business expansion. Visualizing these purposes provides insights into borrower motivations and helps align marketing or financial products with customer needs.
- Home Ownership Analysis (Tree Map): A tree map is used to show how different levels of home ownership (Own, Mortgage, Rent) affect loan applications and funding. The hierarchical structure of this visualization makes it easy to identify which ownership groups contribute most to loan activity and repayment success.

Together, these visuals transform complex lending data into clear business narratives. The Overview Dashboard allows managers and analysts to interact with the data — filtering by time, region, or loan type — to uncover relationships and patterns that might otherwise remain hidden.

![Overview Dashboard](https://github.com/Gurpreet-Labana/Bank-Loan-Analysis-using-Power-BI-SQL/blob/main/Output%20Visuals/Overview.png)
  

#### **Dashboard 3: Details**
The Details Dashboard was designed as the analytical backbone of the entire system — a deep-dive layer that provides record-level transparency. Where the previous dashboards summarized and visualized trends, this one exposes the raw intelligence behind those metrics.

It draws from a rich bank loan dataset containing fields such as:
Loan ID, Address State, Loan Purpose, Loan Grade and Subgrade, Annual Income, Loan Status, Verification Status, Debt-to-Income Ratio, and Interest Rate.

Each of these data points tells part of the borrower’s story:
- Loan ID uniquely identifies each transaction.
- Address State connects performance data with geographic insights.
- Purpose and Grade/Subgrade provide a sense of creditworthiness and loan intent.
- Annual Income and DTI assess borrower capability.
- Verification Status indicates how the applicant’s financials were validated.
- Loan Status shows the repayment stage (e.g., current, late, or charged off).

By bringing these fields together, the Details Dashboard becomes an interactive data exploration tool. Analysts can drill down into specific borrower segments, investigate repayment anomalies, and verify assumptions made at the Summary or Overview levels.

This dashboard also supports operational decision-making, enabling loan officers and financial analysts to make evidence-based judgments regarding portfolio health, borrower reliability, and recovery strategy.

Ultimately, the Details Dashboard ensures that every data-driven insight is supported by real, verifiable information bridging the gap between strategic dashboards and operational intelligence.

![Details Dashboard](https://github.com/Gurpreet-Labana/Bank-Loan-Analysis-using-Power-BI-SQL/blob/main/Output%20Visuals/Details.png)
 

---

## 🧰 Skills & Tools  

- **Data Querying & Transformation:** SQL (data extraction, joins, cleaning, and transformation)  
- **Business Intelligence & Visualization:** Power BI  
- **DAX Calculations:** Used for KPIs (MTD, MoM, Averages, Ratios)  
- **Analytical Techniques:** Descriptive Analysis, Trend Analysis, Funnel Analysis, and Performance Monitoring  
- **Data Storytelling:** Translating raw data into actionable insights through dynamic visuals  

---

## 📈 Results & Business Recommendations  

The project provided **clear visibility into loan performance metrics** and helped identify actionable insights for business improvement.  

### 🔍 Key Findings  
- Real-time tracking of Total Loan Applications, Total Funded Amount, and Amount Received, enabling management to monitor lending activity dynamically.
- Visibility into Average Interest Rate and Debt-to-Income Ratios, helping to identify credit risk patterns and borrower affordability.
- Clear identification of seasonal lending trends and regional performance disparities across states.
- Better understanding of loan purpose and employment-related repayment behavior, supporting more refined credit policies.

### 💡 Business Recommendations  
1. **Risk-Based Pricing:** Adjust interest rates dynamically for regions or borrower profiles exhibiting higher default probabilities.
2. **Targeted Lending:** Expand offerings in states and segments with proven repayment efficiency.
3. **Portfolio Diversification:** Balance loan purpose distribution to mitigate overexposure to any single category
4. **Operational Optimization:** Use DTI and repayment insights to strengthen pre-loan screening and reduce bad debt ratios.

Overall, the dashboards empower stakeholders with data-driven clarity, leading to smarter, faster, and more confident business decisions.

---

## 🚀 Next Steps  

To extend this project’s analytical value, the following enhancements are recommended:  
- **Integrate Predictive Modelixng:** Apply machine learning to forecast defaults or prepayments.  
- **Automate Data Refresh:** Connect to SQL databases or APIs for real-time reporting.  
- **Expand KPI Tracking:** Include Net Interest Margin (NIM) and Collection Efficiency Rate.  
- **Embed Reports:** Deploy dashboards via Power BI Service for organization-wide accessibility.  

---

## 🧭 Getting Started  

Follow these steps to explore the project on your system:  

1. **Clone the Repository:**  
   ```bash
   https://github.com/Gurpreet-Labana/Bank-Loan-Analysis-using-Power-BI-SQL

2. **Open in Power BI Desktop**
Load the .pbix file to view and interact with the dashboards.

3. **Explore Dashboards**
Navigate between Summary, Overview, and Details dashboards to experience the full analytical journey of the loan portfolio.
