# Data Warehousing Data Mining

### Need for data warehousing

- Centralization of data: A data warehouse enables the consolidation of data from multiple sources into a single repository, providing a centralized location for all data related to an organization. This allows for easier access to data, eliminates redundancy and duplication, and ensures that everyone in the organization is working with the same version of the data.

- Support for business intelligence: A data warehouse provides the foundation for business intelligence (BI) activities, such as reporting, data analysis, and data mining. By centralizing and organizing data, a data warehouse makes it easier to generate insights and draw conclusions from large volumes of data.

- Historical analysis: A data warehouse stores data over an extended period, allowing for the analysis of historical data trends and patterns. This helps organizations understand how their business has evolved over time and identify potential future trends.

- Scalability: A data warehouse is designed to handle large volumes of data and provide fast access to that data. This makes it easier for organizations to grow and scale their operations without having to worry about their data infrastructure.

- Improved decision-making: By providing timely and accurate data, a data warehouse can help organizations make better-informed decisions. With the ability to access and analyze data quickly, decision-makers can respond faster to changing business conditions and make more informed decisions.

- Integration with other systems: A data warehouse can be integrated with other systems, such as customer relationship management (CRM) or enterprise resource planning (ERP) systems, to provide a complete view of an organization's data. This integration allows for a more comprehensive understanding of the business and can help identify areas for improvement.

Overall, data warehousing is crucial for organizations that need to manage and analyze large volumes of data to support their business operations and decision-making.


### Operational & informational data

#### Operational Data: 

- Operational data refers to the data that is generated from day-to-day operations of an organization. This data is usually transactional in nature and is used to support the daily activities of the business. Examples of operational data include sales transactions, inventory levels, customer orders, and employee payroll information.

- Operational data is typically stored in an operational database, which is optimized for transactional processing and is designed to support the high volume of transactions that occur on a daily basis. Operational databases are optimized for fast inserts, updates, and deletes, and are generally not designed for complex analysis or reporting.

#### Informational Data:

- Informational data, on the other hand, refers to the data that is stored in a data warehouse to support analytical processing and reporting. This data is often aggregated and summarized to provide insights into the overall performance of the organization.

- Informational data is usually sourced from multiple operational databases and is transformed and loaded into a data warehouse. The data warehouse is optimized for analytical processing and is designed to support complex queries and reporting. Examples of informational data include sales trends, customer demographics, and product performance.

#### Difference:

- Purpose: Operational data is used to support day-to-day operations, while informational data is used to support analytical processing and reporting.

- Source: Operational data is sourced directly from the operational systems that support the daily activities of the organization, while informational data is sourced from multiple operational systems and is often transformed and aggregated to provide a more complete view of the organization.

- Structure: Operational data is typically transactional in nature and is stored in an operational database, which is optimized for transactional processing. Informational data, on the other hand, is often summarized and aggregated and is stored in a data warehouse, which is optimized for analytical processing and reporting.

- Access: Operational data is accessed by the operational systems and applications that support the day-to-day activities of the organization. Informational data is accessed by business analysts and other users who need to perform complex analysis and reporting on the data.

- Time horizon: Operational data is typically more current and focuses on the short-term, while informational data covers a longer time horizon and provides a more historical perspective on the performance of the organization.

- Granularity: Operational data tends to be more granular and detailed, focusing on individual transactions and events. Informational data, on the other hand, is often aggregated and summarized to provide a higher-level view of the organization's performance.

- Processing: Operational data is processed in real-time or near-real-time to support immediate decision-making and response to events as they occur. Informational data, on the other hand, is typically processed in batch mode, allowing for more complex analysis and reporting over longer time periods.

- Security: Operational data is often subject to stricter security requirements and access controls to ensure the integrity and confidentiality of the data. Informational data is often more widely accessible to users across the organization for reporting and analysis purposes.

- Performance: Operational data systems are designed for high performance and low latency to support real-time processing and decision-making. Informational data systems, on the other hand, are optimized for complex analytical processing, which can be more resource-intensive and time-consuming.

- Volume: Operational data tends to have a higher volume, as it is generated by numerous transactions occurring on a daily basis. Informational data, however, is typically stored in a data warehouse, where it can be aggregated and summarized, reducing the overall volume of data.

- Timeliness: Operational data needs to be available in real-time or near real-time to support the day-to-day operations of the organization. Informational data, however, does not have the same timeliness requirements and can be updated and loaded into the data warehouse on a less frequent basis, such as daily or weekly.

- Purpose of Analysis: Operational data is used to monitor and manage the day-to-day operations of the organization, while informational data is used to provide insights into overall performance and to support strategic decision-making.

- User groups: Operational data is typically used by employees who are involved in the daily operations of the organization, such as sales representatives, customer service agents, and production workers. Informational data, on the other hand, is often used by business analysts, managers, and executives who are responsible for making strategic decisions and managing the overall performance of the organization.

## Data Warehouse definition and characteristics

A data warehouse is a large, centralized repository of integrated data that is specifically designed to support business intelligence (BI) activities such as reporting, analytics, and data mining. It is a system used for storing and managing data from a variety of sources, such as operational systems, external sources, and other data warehouses.

Here are some characteristics of a data warehouse:

- Integrated: A data warehouse integrates data from various sources and formats into a single, consistent format.

- Time-variant: A data warehouse stores historical data that is used to track changes over time and to support trend analysis.

- Subject-oriented: A data warehouse is organized around specific subject areas, such as sales, inventory, or customers.

- Non-volatile: A data warehouse is a read-only system that does not allow data to be modified, ensuring the integrity of the data.

- Large-scale: A data warehouse can store vast amounts of data, ranging from terabytes to petabytes.

- Optimized for queries: A data warehouse is optimized for fast query performance, enabling users to analyze data quickly and efficiently.

- Designed for business intelligence: A data warehouse is specifically designed to support BI activities such as reporting, analytics, and data mining, providing users with the insights they need to make informed business decisions.

- Cleansed and transformed data: Data in a data warehouse is typically cleaned, transformed, and standardized before being loaded into the warehouse. This process ensures data quality and consistency across the organization.

- Decoupled from operational systems: Data warehouses are typically separate from the operational systems that produce the data. This decoupling allows for more efficient querying and reporting on the data, without impacting the performance of operational systems.

- Schema-on-write: In a data warehouse, the schema is defined and applied at the time data is loaded, rather than at the time it is queried. This approach enables faster querying and more efficient storage of data.

- Federated data: In some cases, data warehouses may integrate data from multiple, separate data sources or data marts, creating a federated data warehouse. This approach enables organizations to better manage and analyze data from disparate sources.

- Metadata-driven: Data warehouses are often heavily reliant on metadata, which is data that describes other data. Metadata is used to manage the data warehouse, document the data, and provide context for users.

- Multi-dimensional: Data in a data warehouse is typically organized into multi-dimensional structures, such as cubes or star schemas. These structures enable users to analyze data across different dimensions, such as time, geography, and product.

- Security and access controls: Data warehouses typically have robust security measures and access controls in place to protect the sensitive data they contain.

- Backups and disaster recovery: Data warehouses are typically backed up regularly and have disaster recovery plans in place to ensure data availability in the event of a system failure or other catastrophe.

## Operational Data Stores

An Operational Data Store (ODS) is a type of database that is designed to support operational or transactional systems, providing near-real-time access to current data for operational reporting and analysis. Unlike a data warehouse, which is optimized for complex queries and historical analysis, an ODS is designed to support day-to-day operational activities such as transaction processing and customer support.

Here are some characteristics of an ODS:

- Near-real-time data: An ODS is designed to support near-real-time data processing, allowing data to be updated and accessed quickly.

- Integrated data: An ODS integrates data from multiple sources, such as transactional systems, operational databases, and external sources, into a single, unified view of the data.

- Granular data: An ODS typically stores data at a more granular level than a data warehouse, providing more detailed information about individual transactions and events.

- Current data: An ODS focuses on current data rather than historical data, providing a more accurate picture of current operational activities.

- Subject-oriented: An ODS is typically organized around specific subject areas, such as customers, products, or orders.

- Small-scale: An ODS is typically smaller in scale than a data warehouse, with a focus on supporting specific operational activities rather than enterprise-wide reporting and analysis.

- Flexible data model: An ODS may use a flexible data model, such as a relational or object-oriented data model, to support different types of data and data structures.

- Limited data transformation: An ODS may perform some limited data transformation, such as data cleansing or validation, but it is not optimized for complex data transformations or data aggregation.

- Real-time data access: An ODS provides real-time data access to support operational reporting and analysis, enabling users to quickly access and analyze current data.

## Architectural components

The architectural components of a data warehouse typically include the following:

- Source systems: The source systems are the operational systems that generate the data that is loaded into the data warehouse. These may include transactional databases, external data sources, and other data warehouses.

- Extraction, Transformation, and Loading (ETL) processes: ETL processes are used to extract data from the source systems, transform it into the required format, and load it into the data warehouse. This may involve data cleansing, data integration, data validation, and other data transformation activities.

- Data warehouse database: The data warehouse database is where the integrated, transformed, and loaded data is stored. It is typically optimized for fast query performance and supports complex analytical queries.

- Metadata repository: The metadata repository stores metadata about the data in the data warehouse, including data definitions, data lineage, data relationships, and other information.

- Business intelligence tools: Business intelligence tools are used to analyze and report on the data in the data warehouse. These may include reporting tools, dashboard tools, data visualization tools, and other BI applications.

- Query tools: Query tools are used to access and query the data in the data warehouse. These may include SQL-based query tools, OLAP tools, and other query tools.

- Data marts: Data marts are smaller, subject-specific data warehouses that are designed to support specific business areas or user groups. Data marts are typically derived from the data in the main data warehouse and are optimized for specific business needs.

- Security and access controls: Security and access controls are used to protect the data in the data warehouse and ensure that only authorized users have access to the data.

- Backup and recovery processes: Backup and recovery processes are used to ensure that the data in the data warehouse is protected and can be recovered in the event of a system failure or other catastrophe.

## Data Preprocessing

Data preprocessing is the process of cleaning, transforming, and preparing raw data for analysis. The purpose of data preprocessing is to ensure that the data is accurate, consistent, and complete, and to remove any errors, inconsistencies, or redundancies in the data.

#### Need of Preprocessing Data

- Data Quality: Raw data is often incomplete, inconsistent, or contains errors, which can negatively impact the accuracy and quality of the results. Data preprocessing techniques such as data cleaning, data integration, and data transformation can help to improve the quality of the data by removing errors and inconsistencies.

- Removing noise: Raw data often contains errors and noise that can be introduced during data collection, such as sensor malfunctions or network errors. Data preprocessing techniques such as smoothing or filtering can remove this noise to obtain more accurate data.

- Data Integration: Data from different sources may have different formats and structures. Data preprocessing can help to integrate data from different sources and convert it into a common format.

- Data Reduction: Large datasets can be time-consuming and computationally expensive to process. Data preprocessing techniques such as data sampling and dimensionality reduction can help to reduce the size of the dataset, making it easier and faster to analyze.

- Data Normalization: Data normalization is the process of scaling numerical data to a common range. This can help to ensure that all data is treated equally during analysis and prevent the dominance of certain features over others.

- Feature Extraction: Data preprocessing techniques such as feature extraction can help to identify the most important features in the dataset, making it easier to understand and interpret the results.

#### Data Cleaning Techniques

Data cleaning is an important step in data mining that involves identifying and correcting errors, inconsistencies, and missing values in the dataset. Here are some common data cleaning techniques used in data mining:

- Removing Duplicates: Duplicate records in a dataset can skew analysis results. Data mining practitioners often remove duplicates to prevent this from happening.

- Handling Missing Values: Missing values can occur when data is not collected, or the data is lost during storage or transmission. Data mining practitioners often use techniques like imputation to fill in missing values.

- Outlier Detection and Removal: Outliers are data points that deviate significantly from the average or expected values. Data mining practitioners often use statistical techniques to detect outliers and remove them from the dataset.

- Data Normalization: Normalization is the process of scaling data to a common range. This is often done to ensure that all variables in the dataset are treated equally during analysis.

- Data Transformation: Data transformation involves converting data from one format to another. Data mining practitioners often use this technique to standardize the format of the data, making it easier to analyze.

- Discretization: Discretization involves converting continuous variables into categorical variables. This can be useful in data mining when analyzing data with large ranges of continuous values.

- Handling Noisy Data: Noisy data refers to data that is erroneous, inconsistent, or random. Data mining practitioners often use smoothing techniques to remove noise from the data.

#### Data Integration and Transformation

Data integration and transformation are two important techniques in data mining that are used to prepare data for analysis.

Data Integration involves combining data from different sources into a single dataset that can be analyzed. This is important because data may be spread across multiple sources and formats, making it difficult to analyze. Data integration involves identifying and resolving conflicts in data formats, attributes, and values, so that the data can be combined and analyzed coherently.

Data Transformation involves converting data from one format or structure to another, with the goal of making it more suitable for analysis. This can involve changing the scale or range of variables, standardizing the format of the data, or converting categorical variables into numerical variables. Data transformation can also include feature selection, which involves selecting the most important variables for analysis, and feature engineering, which involves creating new variables that are derived from existing ones.

Data integration and transformation are often used together in data mining, as data integration often requires data transformation to ensure that the data is consistent and suitable for analysis. For example, if two datasets have different scales for the same variable, data transformation may be necessary to standardize the variable before the data can be integrated.

## Data Reduction Techniques 
## Discretization

Unit II

OLAP in the Data Warehouse: [10 Hrs]
A Multidimensional Data Model, Schemas for 
Multidimensional Databases: Stars, Snowflakes, Star join 
and Fact Constellations Measures, Concept Hierarchies, 
OLAP Operations in the Multidimensional Data Model, 
Need for OLAP, OLAP tools , Mining Multimedia 
Databases, Mining Text Databases, Mining the World 
Wide Web.

# Agile

Basics and Fundamentals of Agile Process Methods, Values 
of Agile, Principles of Agile, stakeholders, Challenges
Agile and Scrum Principles: Agile Manifesto, Twelve 
Practices of XP, Scrum Practices, Applying Scrum. Need of 
scrum, working of scrum, advanced Scrum Applications, 
Scrum and the Organization, scrum values


Unit-2 

Agile Product Management
Communication, Planning, Estimation Managing the 
Agile approach Monitoring progress, Targeting and 
motivating the team, Managing business involvement, 
Escalating issue. Quality, Risk, Metrics and 
Measurements, Managing the Agile approach 
Monitoring progress, Targeting and motivating the 
team, Managing business involvement and Escalating 
issue for Agile project management




# Basic Cloud Computing Essentials
# Cloud Security & Migration



