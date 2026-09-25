# Logistic Analytics Project

## Project Overview

This project is a Databricks-based transportation and fleet analytics solution designed to analyze logistics operations using PySpark and a Medallion Architecture.

The project processes transportation data through Bronze, Silver, and Gold layers and generates business insights related to drivers, routes, fleet utilization, maintenance, fuel efficiency, customers, safety, and seasonal patterns.

## Objectives

- Analyze driver performance
- Identify route profitability
- Measure fleet and truck utilization
- Analyze maintenance costs and vehicle downtime
- Monitor fuel efficiency and fuel costs
- Analyze customer revenue and service levels
- Track safety incidents and preventable accidents
- Identify seasonal and monthly transportation patterns

## Architecture

```text
Raw CSV Data
     |
     v
Bronze Layer
     |
     v
Silver Layer
     |
     v
Gold Layer
     |
     v
Business Analysis & Visualizations
```

## Medallion Architecture
## Bronze Layer

Loads the raw transportation datasets into Databricks.

## Silver Layer

Cleans and prepares the data.
Standardizes data types and structures.
Creates analysis-ready Silver tables.

## Gold Layer

Creates business-level analytical tables.
Performs aggregations and joins.
Supports business questions and visualizations.
Technologies Used
Databricks
PySpark
Python
Delta Lake
GitHub
Databricks Notebooks
Medallion Architecture

## Project Notebooks
| Notebook                     | Analysis                                     |
| ---------------------------- | -------------------------------------------- |
| 01_Bronze_Layer              | Raw data ingestion                           |
| 02_Silver_Layer              | Data cleaning and transformation             |
| 03_Gold_Driver_Performance   | Driver performance analysis                  |
| 04_Gold_Route_Profitability  | Route profitability analysis                 |
| 05_Gold_Fleet_Utilization    | Fleet utilization analysis                   |
| 06_Gold_Maintenance_Analysis | Maintenance and downtime analysis            |
| 07_Gold_Fuel_Efficiency      | Fuel efficiency and fuel cost analysis       |
| 08_Gold_Customer_Analysis    | Customer revenue and service-level analysis  |
| 09_Gold_Safety_Metrics       | Safety incidents and accident analysis       |
| 10_Gold_Seasonal_Patterns    | Monthly and seasonal transportation patterns |

## Business Questions
1. Driver Performance:
How is each driver performing in terms of on-time delivery rate, MPG, and revenue generated per mile?

2. Route Profitability:
Which routes or lanes are most and least profitable based on revenue versus operating costs?

3. Fleet Utilization:
How effectively is each truck or asset being utilized based on miles driven and revenue generated per asset?

4. Maintenance Analysis:
What is the maintenance cost per mile, and how does vehicle downtime impact fleet operations and profitability?

5. Fuel Efficiency:
How does fuel efficiency (MPG) trend over time, and which routes have the highest and lowest fuel costs?

6. Customer Analysis:
How much revenue is generated from each customer, and how well are customer service-level requirements being met?

7. Safety Metrics:
What are the incident rates and number of preventable accidents by driver, vehicle, route, or time period?

8. Seasonal Patterns
How do load volumes and freight rates fluctuate across different seasons, months, or periods?

## Key Gold Tables

- `gold_driver_performance`
- `gold_route_profitability`
- `gold_fleet_utilization`
- `gold_maintenance_analysis`
- `gold_fuel_efficiency`
- `gold_customer_analysis`
- `gold_safety_metrics`
- `gold_seasonal_patterns`

## Data Pipeline

The project follows this workflow:

```text
Raw Transportation Data
          |
          v
Bronze Tables
          |
          v
Silver Tables
          |
          v
Gold Analytical Tables
          |
          v
Business Insights
```

## Key Analysis Areas
## Driver Performance

Analyzes:

- Total trips
- Total miles
- Total revenue
- On-time delivery rate
- MPG
- Revenue per mile
- Route Profitability

## Route Profitability
Analyzes:

- Total loads
- Revenue
- Fuel cost
- Profit
- Profit per mile
- Fleet Utilization

## Fleet Utilization
Analyzes:

- Trips completed
- Miles driven
- Revenue
- Utilization rate
- MPG
- Maintenance cost
- Downtime
- Maintenance

## Maintenance Analysis
Analyzes:

- Maintenance events
- Maintenance cost
- Maintenance cost per mile
- Downtime
- Fuel Efficiency

## Fuel Efficiency
Analyzes:

- MPG over time
- Fuel consumption
- Fuel cost by route
- Distance traveled
- Customer Analysis

## Customer Analysis
Analyzes:

- Customer revenue
- Number of loads
- On-time deliveries
- Detention time
- Safety

## Safety Metrics
Analyzes:

- Total incidents
- Preventable accidents
- At-fault incidents
- Injury incidents
- Vehicle and cargo damage
- Incident rates
- Seasonal Patterns

## Seasonal Patterns
Analyzes:

- Monthly load volume
- Monthly revenue
- Freight rate per mile
- Seasonal load volume
- Seasonal freight rates

## Data Visualization
Databricks visualizations are used to present:

- Driver revenue and delivery performance
- Route profitability
- Fleet utilization
- Maintenance cost and downtime
- Fuel efficiency trends
- Customer revenue and service levels
- Safety incidents
- Monthly and seasonal transportation patterns

## Project Outcome
The project demonstrates how Databricks and PySpark can be used to build an end-to-end transportation analytics pipeline using the Medallion Architecture.

The final Gold layer provides business-ready datasets that can be used to understand transportation performance, fleet operations, maintenance, fuel efficiency, customer service, safety, and seasonal trends.

Author

Shravya
