# Intermediate_Assessment_Codeathon
Logistics and Transportation - Fleet Performance and Delivery Efficiency

## Project Overview

This project focuses on analysing fleet performance and delivery efficiency for a logistics and transportation company using Microsoft Excel, Power Query and Power BI.

The objective is to evaluate delivery performance, fuel efficiency and operational costs to support better fleet utilisation and route optimisation.

## Problem Statement

A logistics company wants to analyse its fleet performance in terms of:
- On-time deliveries
- Fuel efficiency
- Cost per kilometre
- Vehicle performance
- Delivery performance across routes

The project aims to transform raw transportation data into meaningful insights through data cleaning, data modelling, DAX calculations and interactive visualisations.

## Dataset Description

The project uses two datasets:

**1. Trip Data**
- Trip ID
- Vehicle ID
- Driver ID
- Origin
- Destination
- Distance (km)
- Fuel Consumed (litres)
- Delivery Status
- Delivery Date

**2. Vehicle Master**
- Vehicle ID
- Vehicle Type
- Capacity
- Maintenance Cost

## Tools and Technologies

- Microsoft Excel
- Power Query
- Microsoft Power BI
- DAX
- GitHub

## Data Cleaning and Transformation

Data preparation was performed using Power Query.

Key activities included:

- Corrected Trip ID column heading and initial trip identifiers.
- Applied Trim and Clean operations where appropriate.
- Replaced invalid distance entries with "Unknown".
- Created a separate numeric distance column for calculations, converting "Unknown" values into null.
- Checked data types, missing values and errors.
- Merged Trip Data with Vehicle Master using Vehicle ID.
- Created a reference query to calculate average fuel consumption by Vehicle ID using Group By.
- Merged the average fuel consumption table back into the trip dataset.
- Created a Fuel Cost column using the assumed fuel price of ₹95 per litre.

**Fuel consumption note:** The original dataset did not contain missing fuel consumption values. Therefore, no existing fuel consumption values were replaced. The average fuel consumption calculation and merge were performed to prepare the replacement logic.

## Data Modelling

The trip data and vehicle master information were combined using Vehicle ID to create a consolidated dataset for analysis.

## DAX Measures

The following measures were created in Power BI:

**1. Fuel Efficiency**

Total Distance / Total Fuel Consumed

**2. On-Time Trips**

Counts the number of trips with On-Time delivery status.

**3. Total Trips**

Counts the total number of trip records.

**4. On-Time Delivery %**

On-Time Trips / Total Trips × 100

**5. Total Fuel Cost**

Sum of Fuel Cost.

**6. Total Maintenance Cost**

Sum of Maintenance Cost.

**7. Total Distance**

Sum of numeric distance values.

**8. Cost per km**

(Total Fuel Cost + Total Maintenance Cost) / Total Distance

## Dashboard and Visualisations

The Power BI report includes the following visualisations:

- KPI cards for key fleet performance measures.
- Clustered bar chart showing On-Time Delivery % by Route.
- Line chart showing Fuel Efficiency trends by Month.
- Map visual showing delivery performance by route using Origin and Destination.
- KPI card for Cost per km.

## Key Learnings

Through this project, I gained practical experience in:

- Data cleaning and transformation using Power Query.
- Merging queries and creating reference queries.
- Group By operations and average calculations.
- Data type conversion and handling unknown values.
- Creating calculated columns and DAX measures.
- Designing Power BI dashboards and visualisations.
- Analysing fleet performance and delivery efficiency.

## Conclusion

This project demonstrates how raw logistics data can be transformed into an analytical dashboard to evaluate delivery performance, fuel efficiency and operational costs.

The resulting analysis provides a foundation for identifying delivery trends, monitoring fleet performance and supporting data-driven operational decisions.
