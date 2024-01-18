# Power BI Analytics Project Readme


## Project Overview

Welcome to the Power BI Analytics project! This project focuses on analyzing and visualizing data from various sources to gain valuable insights into business operations. In this readme file, we'll guide you through the initial steps of the project, specifically the downloading, importing, and transformation of data within the following tables: Orders, Products, Sales, and Customers.


## Table of Contents

1. [Data Sources](#data-sources)
2. [Importing Data](#importing-data)
3. [Data Transformation](#data-transformation)
4. [Creating a Data Model](#Creating-a-data-model)
5. [Setting up the Report](#Setting-up-the-report)

## Data Sources

The project relies on four key tables: Orders, Products, Sales, and Customers. Each table provides essential information that contributes to a comprehensive understanding of the business data.

- **Orders:** Contains details about each order, including the order and shipping dates, the customer, store and product IDs for associating with dimension tables, and the amount of each product ordered.

- **Products:** Encompasses information about each product sold by the company, including the product code, name, category, cost price, sale price, and weight.

- **Stores:** Contains information on each store, including the store code, store type, country, region, and address.

- **Customers:** Stores customer-related information, including customer ID, name, and geographical location.


## Importing Data

To kickstart the project, I initally imported the each table, in a variety of ways. These include from: an azure database, a csv file, a blob storage and also a zip file.

## Data Transformation

Once the data was imported, I performed  necessary transformations using the power query editor tool. Using this I deleted uneccessary columns, created new columns using DAX formulas, split collumns into two new columns (e.g. splitting full name in first name and last name), removed null values and changed  missing values to the average for that column.


## Creating a data model

For this task I created a date table, a star schema, a measures table with key measures such as Total Profit and also date a geography hierachies.


## Setting up the Report

After completing these tasks I then set up my report by creatig the following pages:
- Executive Summary
- Customer Detail
- Product Detail
- Stores Map

I added a navigation bar to each of these pages.


## Building the Customer Report page

Within  the customer report page I created:
- Card visuals
- A line chart of weekly distinct customers
- A table showing the top 20 customers by revenue
- A donut chart showing the number of customers by country
- A date slicer


## Building the Executive Summary page

Within this page I created:
- Card visuals showing total revenue, total profit and total orders
- A graph of revenue against time
- Donut charts showing orders and revenue by country
- A bar chart of orders by category
- KPIs for quarterly revenue, customers and profit
- A table of the top 10 products


## Building the Product Detail page

Within this page I created:
- Gauge visuals showing performances compared to quarterly targets
- An area chart
- A table of the top 10 products in the selected context
- A scatter graph


## Building the Stores Map page

Within this page I created:
- A map visual allowing you to see where stores are located, where you can hover over them and see how they are performing using a drillthrough
