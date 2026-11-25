# Customer Segmentation Using RFM Analysis

## Project Overview

This project develops an end-to-end customer segmentation pipeline using a retail transactions dataset containing over **44,000 records**.

The main objective is to transform raw transactional data into meaningful customer insights by identifying groups of customers based on their purchasing behaviour. These insights can help businesses understand customer value, improve retention strategies, and make more informed marketing decisions.

## Objectives

- Clean and prepare raw retail transaction data for analysis.
- Engineer customer-level features from transactional records.
- Segment customers using Recency, Frequency, and Monetary (RFM) analysis.
- Prepare customer features for potential clustering through log transformation and standardization.
- Identify valuable customer segments and analyse their contribution to revenue.

## Methodology

### 1. Data Cleaning and Preparation

The raw dataset was cleaned and validated to improve data quality and ensure reliable analysis.

The cleaning process addressed:
- Missing customer IDs.
- Duplicate transactions.
- Cancelled transactions.
- Invalid prices and quantities.
- Non-product transaction codes.
- Extreme outliers.

A cleaning log was maintained to account for removed records and document the data preparation process.

### 2. Feature Engineering

Transactional records were transformed into customer-level features to capture purchasing behaviour.

The analysis focused on three key RFM metrics:

| Metric | Description |
|---|---|
| **Recency** | How recently a customer made a purchase. |
| **Frequency** | How frequently a customer made purchases. |
| **Monetary** | How much a customer spent. |

### 3. Customer Segmentation

RFM scoring was applied to evaluate customers across the three metrics and classify them into meaningful segments based on their purchasing behaviour.

The resulting customer groups provide a clearer understanding of customer engagement and value.

### 4. Feature Transformation and Scaling

To prepare the customer-level feature matrix for clustering, I applied:
- Log transformation to reduce skewness in the feature distributions.
- Standardization to bring numerical features onto comparable scales.

These steps prepared the data for further clustering analysis.

## Key Findings

The analysis identified **1,500 customers** and revealed a significant difference in revenue contribution across customer segments.

<blockquote>
  **Champions Segment**

  - 12.7% of customers
  - 45% of total revenue
</blockquote>

Despite representing a relatively small proportion of the customer base, Champions generated nearly half of the total revenue.

This highlights the importance of identifying and retaining high-value customers.

## Technologies Used

- **Python** – Data processing and analysis.
- **Pandas** – Data cleaning, manipulation, and aggregation.
- **NumPy** – Numerical operations and feature transformations.
- **Data Visualization** – Exploring customer behaviour and segment distributions.

## Business Value

The project demonstrates how transactional data can be transformed into actionable business insights. Businesses can use these segments to:

- Prioritize high-value customers through loyalty and retention strategies.
- Identify customers who may need targeted engagement.
- Develop more focused marketing campaigns.
- Better understand purchasing patterns and revenue distribution.

## Conclusion

This project strengthened my understanding of the data preparation and feature engineering stages that underpin reliable data-driven solutions. It also demonstrated how customer analytics can bridge technical data processing and practical business decision-making.
