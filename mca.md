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

#### Difference

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

. Architectural components, Data 
Preprocessing: Need of Preprocessing Data, Data 
Cleaning Techniques, Data Integration and 
Transformation, Data Reduction Techniques, 
Discretization

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



