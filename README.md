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
- Key KPIs: total orders, on-time delivery rate, average delivery time, average customer satisfaction (CSAT), number of drivers, number of hubs  
- Visuals include: line, bar, column and scatter plot to represent order trends, hub utilization, driver performance, fleet reliability, and workload distribution
- Interactivity: slicers for Year, Hub, Driver, Vehicle, Delivery Status, and CSAT score

--- 
## Key Findings
1. Freightliner M2 records both the highest number of breakdowns and the highest count of Order IDs, indicating it is the most frequently used vehicle, while Chevrolet Express records the lowest breakdowns and Ford F-150 records the lowest Order IDs.
2. Vehicle code FT-010 is associated with the highest sum of breakdowns, indicating it requires the most attention in terms of maintenance and reliability.
3. From 2018 to 2023, October records the highest sum of breakdowns while September records the lowest, indicating a seasonal pattern in vehicle reliability.
4. Vehicles from 2019 show higher breakdowns than those from 2018, suggesting that breakdowns are influenced not only by age but also by factors such as usage and maintenance.
5. While smaller hubs like Dallas handle a high number of orders efficiently, Houston, despite having high capacity, processes fewer orders, suggesting underutilization.
6. Orders vary by month, with May recording the highest number of orders and February the lowest, indicating peak demand around May and lower activity in February.
7. Most vehicles are active, with 33 (73.33%) in active status, while 12 are either needing maintenance or marked as draft, indicating the fleet is largely operational but some vehicles require attention.
8. Vans account for approximately 62.48% of total Order IDs, making them the most utilized vehicle type, while box trucks account for about 4.4%, indicating the lowest usage among vehicle types.
9. Christopher Martin records the highest number of Order IDs and the highest count of delayed deliveries among all drivers, indicating a need for closer monitoring or support to improve timeliness.
10. Less experienced drivers (1–2 years) show wide variability in ratings, while from 3+ years onward, lower ratings disappear and scores stabilize between 3–5. Highly experienced drivers (10 years) consistently achieve the highest ratings (4–5), indicating stronger and more reliable performance.


--- 
## Recommendations 
1.	Improve fleet availability tracking: Maintain and regularly update vehicle status (active, maintenance, draft) to ensure maximum fleet readiness and reduce downtime.
2.	Strengthen preventive maintenance strategy: Use breakdown trends by year (e.g., higher breakdowns in 2019 vehicles) to schedule proactive maintenance rather than reactive repairs.
3.	Address seasonal and monthly demand patterns: Plan fleet capacity and staffing around peak months like May and high breakdown periods like October to avoid service disruptions.
4.	Leverage experienced drivers: Assign high-priority or time-sensitive deliveries to more experienced drivers (5+ years) who demonstrate more consistent high ratings.
5.	Implement driver training programs: Focus on supporting less experienced drivers (1–2 years) to reduce performance variability and improve consistency in ratings.
6.	Enhance driver performance monitoring: Closely monitor drivers with high delays, such as Christopher Martin, and provide targeted training or support to improve delivery timeliness.
7.	Reallocate vehicle usage: Increase use of underutilized vehicle types like box trucks where appropriate, and ensure optimal assignment of vans since they handle the majority of orders.
8.	Optimize fleet utilization: Investigate underutilization in hubs like Houston and redistribute workloads or routes to better balance order distribution across hubs.
9.	Improve maintenance for high-risk vehicles: Prioritize regular inspections and preventive maintenance for Freightliner M2 and vehicle code FT-010, as they record the highest breakdowns and usage.


 
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
4.	Use slicers and filters to interact with the visuals and drill down into years or drivers
5.	Review KPI cards, charts, and tables to understand trends, performance metrics, and operational insights.
 

  
--- 
 
## Contact 
Babra Odongo
odongobabra5@gmail.com
https://www.linkedin.com/in/babra-odongo-047921268/



