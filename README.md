# 📊 Data Analysis Project with SQL

Welcome! This repository showcases a complete **Data Analysis workflow using SQL**, starting from **Exploratory Data Analysis (EDA)** and moving toward **Advanced Analytics** with reports, metrics, and trend analysis.  

The goal of this project is to **demonstrate how SQL can be used as the primary tool for data exploration, segmentation, and business performance evaluation**.  

---

## 📑 Table of Contents
1. [Workflow Diagram](#-workflow-diagram)  
2. [Exploratory Data Analysis (EDA)](#1-exploratory-data-analysis-eda)  
3. [Advanced Analytics](#2-advanced-analytics)  

---

## 🗂️ Workflow Diagram

![image](https://github.com/user-attachments/assets/622e7622-921b-457b-b8d6-f0bbc6b9a2a8)  


The workflow is divided into two main phases:  
1. **EDA (Exploratory Data Analysis)** – Steps 1 to 9.  
2. **Advanced Analytics** – Steps 10 to 12.  

---

## 1️⃣ Exploratory Data Analysis (EDA)

The **EDA** phase provides an initial understanding of the dataset, validates its quality, and identifies patterns or inconsistencies.  

Key stages include:  
- **Database Exploration** → Inspecting tables and columns with `INFORMATION_SCHEMA`.  
- **Dimensions Exploration** → Analyzing customers, products, and categories.  
- **Data Exploration** → Detecting outliers and missing values.  
- **Measures Exploration** → Calculating KPIs (`SUM`, `COUNT`, `AVG`).  
- **Magnitude Analysis** → Evaluating sales or customer volume by category/country.  
- **Ranking (Top N / Bottom N)** → Identifying best/worst customers or products using window functions.  
- **Reporting** → Creating analytical views (e.g., `report_customers`, `report_products`).  
- **Data Segmentation** → Using `CASE WHEN` to classify customers (VIP, Regular, New).  
- **Part-to-Whole Analysis** → Measuring contribution of each category to the total (%).  

---

## 2️⃣ Advanced Analytics

This phase applies specialized techniques to analyze **performance, trends, and time evolution**:  

- **Performance Analysis** → Comparing YoY and MoM metrics using `LAG` / `LEAD`.  
- **Cumulative Analysis** → Tracking cumulative totals and moving averages (`SUM() OVER`).  
- **Change-Over-Time (Trends)** → Understanding seasonal patterns by grouping data (month, quarter, year).  

---
