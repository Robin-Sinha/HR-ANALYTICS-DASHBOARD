HR Analytics Dashboard

Project Overview

This project is an HR Analytics Dashboard built in Microsoft Power BI to understand employee attrition and identify the factors that may be associated with employees leaving the company.

The dashboard brings together employee information such as age, gender, education, salary, job role, satisfaction and years spent at the company. The aim is to present the data in a simple way so that HR teams can quickly understand where attrition is higher.

Business Objective

Main question:

What are the important factors associated with employees leaving the company?

The dashboard allows users to look at attrition from different perspectives and compare employee groups.

Tools Used

Microsoft Power BI

Power Query

DAX

Excel / CSV

Power Query was used for data cleaning and transformation while DAX was used to create the required measures and KPIs.

Dashboard

KPIs

Total Employees

Attrition

Attrition Rate

Average Age

Average Salary

Average Years at Company

Department Slicer

Human Resources

Research and Development

Sales

Main Visualizations

Attrition by Education

Attrition by Age

Attrition by Job Role

Attrition by Job Role and Satisfaction Rating

Attrition by Salary

Attrition by Years at Company

Attrition by Gender

Data Cleaning and Transformation

The data was prepared using Power Query. The main steps included:

checking null values

removing unwanted rows

checking duplicate records

standardizing values

setting correct data types

creating required columns

An Attrition Count column was created to convert Yes and No attrition values into numeric values for aggregation.

A calculated column was also created for Job Satisfaction Rating. The original numeric ratings were converted into meaningful categories:

1 = Low

2 = Medium

3 = High

4 = Very High

The satisfaction rating column was then sorted using a custom sort order so that the categories appear correctly as Low, Medium, High, and Very High instead of being arranged alphabetically.

DAX

The dashboard uses DAX measures for the main KPIs and calculations.

Attrition Rate =
DIVIDE(
    SUM('Employee'[Attrition Count]),
    [Employee Count]
)

The Attrition Rate measure was formatted as a percentage.

Other KPIs include employee count, average age, average monthly income, and average years at company.

Dashboard Theme and Design

A custom theme was applied to the dashboard to maintain a consistent visual style across all pages and visuals.

The dashboard uses a dark themed layout with consistent formatting, colors, cards, slicers and visual styling. The theme was used to make the dashboard look more professional and keep the different visuals visually consistent.

The one-page layout was organized into:

Top-level KPIs

Department slicer

Demographic analysis

Employee experience and satisfaction

Compensation and job role analysis

The goal was to keep the dashboard simple and easy to understand for non-technical stakeholders.

Key Insights

Overall attrition rate is 16.1%.

The 26 to 35 age group has the highest attrition count.

The lowest salary band up to 5K has the largest number of exits.

Laboratory Technicians have the highest attrition count among the job roles shown.

Male attrition is higher than female attrition in the overall dashboard.

Education and satisfaction provide additional perspectives for understanding attrition.

A higher attrition count does not necessarily mean that a group has the highest attrition rate so the metrics should be interpreted in context.

Project Structure

HR-Analytics-Dashboard/
|
├── HR Analytics Dashboard.pbix
├── README.md
└── Data/
    └── HR Analytics.csv

What I Practiced

importing data into Power BI

cleaning and transforming data with Power Query

creating calculated and conditional columns

creating custom categories for satisfaction ratings

applying custom sorting

creating DAX measures

building KPI cards

using slicers

selecting appropriate visualizations

applying a custom Power BI theme

formatting a one-page dashboard

identifying and presenting business insights

cross-checking results

Project Type

This is a guided Power BI project completed by following a structured tutorial and applying the concepts in Power BI. The project was created to get practical experience with the complete dashboard development workflow.

About the Project

This was a guided Power BI project to understand the complete workflow from data cleaning to visualization and analysis. It provided practical experience with Power Query, DAX, calculated columns, custom sorting, Power BI visuals, dashboard themes, dashboard design and business-focused presentation.
