# **Data WareHouse**
---
# Abstraction :



In this paper, then, we describe a few approaches that are being developed, including virtual data warehouses or enterprise portals that support access through views or links directly to the operational data sources. In this architecture, data flows continuously into a data warehouse, and is staged into one or more OLAP tools that are used as computation engines to continuously and incrementally build summary data cubes, which might then be stored back in the data warehouse. Analysis and data mining functions are performed continuously and incrementally over these summary cubes. Retirement policies define when to discard data from the warehouse.


# Introduction:
## what is data warehouse ?


**Data Warehouse modeling is the process of building a model for the data that is to be stored in the data warehouse. The model produced is an abstract model, and in this sense, it is a representation of reality, or at least a part of reality which the data warehouse is assumed to support.** Data Warehouse (DW) is a relational database that is designed for query and analysis rather than transaction processing. It includes historical data derived from transaction data from single and multiple sources. A Data Warehouse provides integrated, enterprise-wide, historical data and focuses on providing support for decision-makers for data modeling and analysis. It is process for collecting and managing data from varied sources to provide meaningful business insights.
A Data Warehouse is typically used to connect and analyze business data from heterogeneous sources. The data warehouse is the core of the BI system which is built for data analysis and reporting. It is a blend of technologies and components which aids the strategic use of data. It is electronic storage of a large amount of information by a business which is designed for query and analysis instead of transaction processing. It is a process of transforming data into information and making it available to users in a timely manner to make a difference.
A Data Warehouse can be viewed as a data system with the following attributes:
* It is a database designed for investigative tasks, using data from various applications.
* It supports a relatively small number of clients with relatively long interactions.
* It includes current and historical data to provide a historical perspective of information.
* Its usage is read-intensive.
* It contains a few large tables.
"Data Warehouse is a subject-oriented, integrated, and time-variant store of information in support of management's decisions."


## Data Warehousing 

- Data Warehousing is the act of **Organizing** & **Storing** data in a way so as to make its retrieval efficient and insightful.
- It's also called as the process of transforming **data** into **information** 

Data Warehousing implements **the process to access heterogeneous data sources, clean, filter, and transform the data and store the data in a structure that is easy to access, understand, and use**. The data is then used for query,reporting, and data analysis. As such, the access, use, technology, and performance requirements are completely different from those in a transaction-oriented operational environment. The volume of data in data warehousing can be very high.


# Architecture of Data Warehouse
![](https://upload.wikimedia.org/wikipedia/commons/8/8d/Data_warehouse_architecture.jpg)

1. **External Sources**
is a source from where data is collected irrespective of the type of data. Data can be structured, semi structured and unstructured as well. 
1. **Stage Area** since the data, extracted from the external sources does not follow a particular format, so there is a need to validate this data to load into datawarehouse. For this purpose, it is recommended to use ETL tool. 
1. **Data-warehouse** after cleansing of data, it is stored in the datawarehouse as central repository. It actually stores the meta data and the actual data gets stored in the data marts. Note that datawarehouse stores the data in its purest form in this top-down approach. 
1. **Data mart** is also a part of storage component. It stores the information of a particular function of an organisation which is handled by single authority. There can be as many number of data marts in an organisation depending upon the functions. We can also say that data mart contains subset of the data stored in datawarehouse. 
1. **Data Mining**
is the practice of analysing the big data present in datawarehouse is data mining. It is used to find the hidden patterns that are present in the database or in datawarehouse with the help of algorithm of data mining. 

This approach is defined by Inmon as datawarehouse as a central repository for the complete organisation and data marts are created from it after the complete datawarehouse has been created. 


# How Data Warehouse works?
A Data Warehouse works as a central repository where information arrives from one or more data sources. Data flows into a data warehouse from the transactional system and other relational databases.

* Structured
* Semi-structured
* Unstructured data

The data is processed, transformed, and ingested so that users can access the processed data in the Data Warehouse through Business Intelligence tools, SQL clients, and spreadsheets. A data warehouse merges information coming from different sources into one comprehensive database. By merging all of this information in one place, an organization can analyze its customers more holistically. This helps to ensure that it has considered all the information available. Data warehousing makes data mining possible. Data mining is looking for patterns in the data that may lead to higher sales and profits.



# Techniques of Data Warehouse
Listed below are the principal modeling techniques that should be arranged into an overall data warehouse modeling approach.
1. Dimensional data modeling.
1. Temporal data modeling.
1. Techniques for building generic and reusable data models (sometimes
referred to as pattern-oriented data modeling). These techniques are much
more extensively and frequently considered in the context of software
development. Data warehouse modelers should learn to apply some of
these techniques, although a transposition from a software development
context to a data warehouse development context may not always be
obvious.
1. Data architecture modeling consists of a combination of top-down enterprise data modeling techniques and bottom-up (detailed) model integration. Data architecture modeling also should provide the techniques for logical data partitioning, granularity modeling, and building multitiered data architectures

# Data Warehouse Tools

There are many Data Warehousing tools are available in the market:

**MarkLogic:**

MarkLogic is useful data warehousing solution that makes data integration easier and faster using an array of enterprise features. This tool helps to perform very complex search operations. It can query different types of data like documents, relationships, and metadata.

https://www.marklogic.com/product/getting-started/

**Oracle:**

Oracle is the industry-leading database. It offers a wide range of choice of data warehouse solutions for both on-premises and in the cloud. It helps to optimize customer experiences by increasing operational efficiency.

https://www.oracle.com/index.html

**Amazon RedShift:**

Amazon Redshift is Data warehouse tool. It is a simple and cost-effective tool to analyze all types of data using standard SQL and existing BI tools. It also allows running complex queries against petabytes of structured data, using the technique of query optimization.

https://aws.amazon.com/redshift/?nc2=h_m1


# Conclusion

Data house is not new phenomenon. All large organization already have data warehouses but they are not just managing them. Over the next few years , the growth of data is going to be enormous with new products and technologies coming out frequently. In order to get the most out of the period , it is going to important that data warehouse planners and devlopers have a clear idea of what they are looking for and then choose strategies and methods that will provide them with performance today and flexibility for tomorrow. Data warehouses and data marts are means for businesses to gather intelligence about their products, customers, and enable them to make informed effective business decisions.The Data Warehouse is responsible for obtaining, cleansing, and organizing data and the data mart functions as the analysis and cataloging center, to create fast and simply information queries.


# References 
1. http://ilpubs.stanford.edu:8090/76/1/1995-10.pdf

1. http://eddyswork.synthasite.com/resources/Data%20Modeling%20Tech%20For%20Data%20Warehouseing.pdf

1. https://www.youtube.com/watch?v=CHYPF7jxlik&t=355s

1. https://www.slideshare.net/KarthikSrini2/data-warehousing-71815590

1. https://www.researchgate.net/profile/Deepak-Sharma-119/publication/358675111_A_Study_on_Inventory_Management_System_A_Case_Study_of_Hindustan_Aeronautics_Limited_HAL_Nashik/links/620e8f4bf02286737ca61984/A-Study-on-Inventory-Management-System-A-Case-Study-of-Hindustan-Aeronautics-Limited-HAL-Nashik.pdf#page=41


