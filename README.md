# Business-Intelligence-Data-Warehousing
 The original dataset can be downloaded from here: https://archive.ics.uci.edu/ml/datasets/Incident+management+process+enriched+event+log

## 1. Data Warehouse Modeling
The goal here is to  present a design of a data warehouse/data mart for an IT Operations Log System. The main executed task were: 

**A. Dataset analysis:**
- Analyze the dataset: Review the fields of the dataset and its definition, understand the meaning of all of them and define user requirements considering the context of the dataset. 
- Detect potential data quality issues such as: missing values, incomplete values, errors. Make a decision for each one of these data quality issues. 
- Detect duplicates. 

**B. Data Warehouse approach selection:**
Select between using a corporate information, multidimensional approach or data vault approach.

**C. Data Warehouse design:**
Identify the entities based on the selected approach (fact tables, dimension tables, and metrics). Implement the design with MySQL Workbench as we did during the sessions.

Attached you will find the full Data Modeling report and the designed DW Schema.

**Tools used:**
- Database: MySQL
- Database Modeling: MySQL Workbench

![DW Star Schema](/1_Data_Warehouse_Modeling/DW_Schema.jpg)

## 2. Data Integration Design
This second part is focused on Data Integration. It consists on designing an one-time historic data load using an ETL (Extraction, Transformation, Loading) tool. That means create an ETL process for each dimension and fact table.

**Deliverables:**

- Data Mapping Report: this document describes the default strategy for extracting data from the source, data mapping process, data quality tracking, and metadata approach. 
- ETL scripts: The collection of ETL processes created with Pentaho Data Integration. 
- ETL Instructions: How to execute the entire data loading process.
- Database backup: after the ETL process has been executed with success.

**Tools used:**

Database: MySQL
ETL Tool: Pentaho Data Integration (ktr format)

![Data Mapping Process](/2_Data_Integration_Design/Mapping1.jpg)

## 3. Incident Management System Dashboard

**Who will use the dashboard?**
- IT Operations Manager: Responsible against the CIO for the Incident Management Platform and groups executing the job.

**What is the decision-making objective of this dashboard?**
Understand the performance of the IT Service Team on a time frame, being able to identify:
- What are the main categories associated with the incidents?
- Is the team complying with the standard SLA?
- Is the team following the guides and standard processes to solve the inicidents?
- Is the team validating the priority level, specially for critical incidents?
- Are the incidents being assigned correctly?
- How does the reassignment count affect the average time to close an incident?
- What are the low performing groups? What is driving this situation?

**What type of content will appear in the dashboard?**
- Main Incident Management KPIs to optimize
- Graphs comparing the composition of the KPIs.

**What level of data aggregation will be required by the audience?**
- Basic level of excel and graph interpretation.
- Capacity to filter the evaluation time (Open date of the ticket)

**Tools used:**
- Tableau

![IMS Dashboard](/3_IMS_Dashboard/IMS.png)
