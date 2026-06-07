# 🚕Yellow_Taxi
## Business Context and Goal
Frequent ride cancellations were leading to revenue loss, reduced customer trust, and inefficient resource utilization. The analysis consists of a Deep-dive into ride cancellations to uncover operational and behavioral factors impacting fulfillment, enabling targeted recommendations to reduce cancellations and enhance customer satisfaction.

## Problem Statement
**Increase Fulfillment across the Platform**

## Table of Contents 
- Exploration of data
- Data Cleaning
- Inisghts
- Recommendations

## North Star Metrics
These are the key metrics which would drive fulfillment of rides
- **rides_cancelled_client** :- number of rides cancelled by the client before or after the captain/driver assignment. 
- **rides_cancelled_system** :- number of rides cancelled by the system due to tech or anyother issue.
- **Average ETA ( per hour )** :- It is the time expected by the customer to receive a ride. 
- **Average Time to Cancellation ( per hour )** :- It is the time taken by the customer to cancel the ride.

### Outcome of North Star Metrics
- For all the metrics above,
  - A downward trend increases the fulfillment ⬆️
  - An upward trend decreases the fulfillment 🔻

# Executive Summary: Why Are Rides Being Cancelled?

## What We Found

Our analysis shows that ride cancellations are not primarily driven by customer behavior or driver preferences. Instead, the underlying issue is a **supply-demand imbalance**, especially during peak commuting hours.

When cancellation trends were analyzed across different times of the day, a clear pattern emerged:

- Ride cancellations peak during office commute hours ( 7 AM to 9 AM ).
- Cancellations increase sharply again after 7 PM.

To understand what was causing these cancellations, we examined the cancellation reasons.

The majority of cancelled rides were found to be **unassigned rides**, meaning customers never received a driver. This suggests that customers are not cancelling because they no longer need the ride; rather, the platform is unable to match demand with sufficient driver supply.

## The Role of ETA

Next, we analyzed the Estimated Time of Arrival (ETA) across different time periods.

During office hours, the average ETA is significantly higher compared to other parts of the day. This indicates that available drivers are stretched thin during peak demand periods.

This behavior aligns with customer expectations. During commute hours, customers are highly time-sensitive and need to reach their workplaces or destinations on time. As waiting times increase, customers become less willing to wait and are more likely to cancel their rides.

To validate this further, we examined rides that were successfully assigned to drivers.

Interestingly, rides with assigned drivers during office hours had the **lowest average ETA**. This indicates that customers are willing to complete their rides when a driver is assigned quickly. However, when ETA increases due to limited driver availability, cancellations rise sharply.

## Customer Behavior Changes Outside Office Hours

The analysis also revealed a shift in customer behavior during late evenings and early mornings.

During these periods, customers appear more tolerant of longer wait times. Unlike office-hour commuters who prioritize speed, customers traveling at night are more focused on reaching home safely and are therefore willing to wait slightly longer for a ride.

As a result, the impact of ETA on cancellations is less severe outside peak commuting hours.

## Root Cause

The evidence consistently points to a single root cause:

**Driver supply is unable to keep pace with customer demand during peak hours.**

This creates a chain reaction:

Demand Surge → Driver Shortage → Higher ETA → Unassigned Rides → Customer Cancellations → Lower Fulfillment Rate



## Insights
- ### Insight 1 :-  Cancellations Are Primarily Supply-Driven
  <img width="2188" height="1222" alt="i1" src="https://github.com/user-attachments/assets/29dd3c96-cf40-4357-9447-15d31bfa4f40" />
  Majority of the cancellations were driven by the non-assignment of captains/drivers

- ### Inisght 2
- ### Insight 3
- ### Insight 4
  
## Recomendations
## Caveats



