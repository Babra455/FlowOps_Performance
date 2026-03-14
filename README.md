# FlowOps Performance
 
**Author:** Odongo Babra 
**Date:** 2025-19-03

--- 
 
## Project Background 
FlowOps Performance is a data analytics project focused on evaluating and improving logistics operations through data-driven insights. It analyzes data from orders, hubs, drivers, and vehicles to track key performance metrics such as order volume, on-time delivery rate, customer satisfaction, and delivery time. The project also examines hub utilization, driver performance, workload distribution, and fleet reliability to identify operational inefficiencies. Insights are presented through interactive Power BI dashboards to support better decision-making and improve overall logistics efficiency.

--- 
 
## Project Objective 
- Analyze month-over-month trends in total orders, on-time delivery rate, customer satisfaction (CSAT), and average delivery time to evaluate operational performance over time.
- Assess hub capacity utilization by comparing the number of orders processed at each hub with its operational capacity to identify overloaded and underutilized hubs.
- Evaluate driver performance by analyzing delivery delay frequency, driver ratings, and years of experience to determine factors influencing delivery efficiency.
- Examine the relationship between driver workload and delivery delays to identify whether workload imbalance contributes to performance issues.
- Analyze fleet reliability by investigating the relationship between vehicle age and breakdown frequency to determine the impact of aging vehicles on operational performance.
- Evaluate breakdown trends across different vehicle models to identify models that may be more prone to mechanical failure.
- Analyze workload distribution across hubs, drivers, and vehicle types to detect operational imbalances and inefficiencies in resource allocation.
- Provide data-driven recommendations to improve delivery efficiency, optimize fleet utilization, reduce delays, and enhance customer satisfaction.

--- 
 
## Datasets 

Vehicles.csv  -  This dataset contains information about the logistics fleet and vehicle condition. It includes columns such as vehicle_id, vehicle_model, purchase_date, vehicle_status, breakdown, maintenance_count_alert, and vehicle_code. The dataset helps analyze fleet reliability, vehicle age, maintenance needs, and breakdown patterns across different vehicle models.

Orders.csv -  This dataset records all delivery transactions and operational activities. It includes fields such as order_id, order_date, actual_delivery_date, order_status, hub_name, driver_id, driver_name, vehicle_name, vehicle_type, delivery_time, hub_processing_time_hours, delay_reason, is_delayed, is_on_time, and customer_satisfaction. It serves as the main dataset for tracking delivery performance, delays, customer satisfaction, and overall logistics efficiency.

Hubs.csv -  This dataset contains information about logistics hubs used for order processing and distribution. It includes columns such as hub_id, hub_name, and hub_capacity. The dataset is used to evaluate hub capacity utilization and identify overloaded or underutilized hubs.

Drivers.csv  -  This dataset contains information about drivers responsible for deliveries. It includes fields such as driver_id, driver_name, employment_type, hire_date, experience_years, and performance_rate. This dataset supports analysis of driver performance, experience levels, and their impact on delivery efficiency and delays.


--- 
## Dashboard Features 
- Key KPIs: total orders, on-time delivery rate, average delivery time, customer satisfaction (CSAT)
- Visuals include: line, bar, column, scatter, and heatmap charts to represent order trends, hub utilization, driver performance, fleet reliability, and workload distribution
- Interactivity: slicers for Date/Month, Hub, Driver, Vehicle, Delivery Status, and CSAT score

--- 
## Key Findings
1.	The hour with the highest number of transaction failures is 13:00, followed by 04:00 and 14:00, while the lowest failures occur at 01:00, 18:00, and 08:00.
2.	 Day 6 records the highest number of failures, followed by Day 4, and Day 2 has the lowest number of failures.
3.	Monthly trends indicate that Month 3 has the highest number of failures, followed by Month 7, whereas Month 2 and Month 9 record the lowest failures.
4.	Status inconsistencies exist across all systems, with the largest mismatches between the app and Banklink, totaling 922, while app–CoralPay mismatches are the lowest at 489.
5.	There are no duplicate utility transactions and no transactions assigned to the wrong provider, indicating that utility transactions are being accurately recorded.
6.	 CoralPay processes a higher number of transactions, including both successful and failed ones, and maintains a high success rate of 81.85%, while NIBSS has the highest number of failed transactions at 7,516, resulting in a failure rate of 20.52%.
7.	Orphaned transactions, which occur when a transaction appears in the system without a corresponding match in partner records, are highest for Banklink at 1,140, with a high total orphaned amount, and lowest for iRecharge at 371 with a lower total amount.
8.	Overall, the total failed transaction amount is 240,524,436.96, with missing amounts in Banklink and NIBSS of 52,653,820.81 and 82,540,011.63 respectively, leading to an average daily loss of 329,485.53 and a total financial exposure of 1,378,399,256.96, highlighting the need for improved monitoring and reconciliation.


--- 
## Recommendations 
1.	Hourly Failures: Implement time-based monitoring and alerts for high-failure hours (13:00, 04:00, 14:00) and consider load balancing or additional system checks during these peak hours to reduce failures.
2.	 Daily Failures: Investigate processes on Day 6 and Day 4 to identify operational or system patterns causing spikes, and establish daily reconciliation routines to catch errors early.
3.	Monthly Failures: Perform monthly trend analysis to understand recurring issues in Months 3 and 7, and schedule preventive system maintenance ahead of high-failure months.
4.	 Status Inconsistencies: Strengthen data reconciliation between the app and Banklink, implement automated mismatch detection, and conduct regular audits to reduce accounting errors and disputes.
5.	 Utility Transactions: Continue strict validation controls to maintain accurate utility transactions, and implement periodic reviews to ensure no duplicate or misassigned transactions occur.
6.	 Provider Performance: Work with NIBSS to improve reliability and reduce failed transactions, while leveraging CoralPay’s high success rate as a benchmark for best practices across providers.
7.	Orphaned Transactions: Implement automated orphan detection and resolution processes, especially for Banklink, to minimize unmatched transactions and improve transaction alignment.
8.	 Financial Exposure: Establish real-time monitoring and alerts for failed and missing transactions, strengthen reconciliation processes, and conduct root-cause analysis to prevent recurring financial losses.


 
--- 
 
## Tools & Techniques 
-	Data Cleaning and Transformation (Power Query)
-	Data Modeling and Relationships
-	DAX Calculations and Derived Metrics
-	Data Visualization and Dashboard Creation
-	Interactive Filtering and Slicers
-	KPI Design and Performance Monitoring

--- 
 
## Project Files (included) 
-	`README.md` — this documentation 
-	`MP_PowerBI_Project_1` – The problem
 
--- 
 
## How to Run / View 
1.	Open `FlowOps Performance `in PowerBI Desktop (recommended)   
2.	Connect to the required data sources if prompted.
3.	Navigate through the dashboard pages to explore different analyses.
4.	Use slicers and filters to interact with the visuals and drill down into hubs, drivers, vehicles, or specific time periods.
5.	Review KPI cards, charts, and tables to understand trends, performance metrics, and operational insights.
6.	Refer to `TransPath Oversight Presentation.pdf` for a summary of insights and recommended actions 

 

 
--- 
 
## Contact 
Babra Odongo
odongobabra5@gmail.com
https://www.linkedin.com/in/babra-odongo-047921268/



