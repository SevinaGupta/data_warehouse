# **Data WareHouse**
---
# Abstraction :


Data warehouses and on-line analytical processing (OLAP)tools have become essential elements of decision support systems. Traditionally, data warehouses are refreshed periodically by extracting, transforming, cleaning and consolidating data from several operational data sources. The data in the warehouse is then used to periodically generate reports, or to rebuild multidimensional (data cube) views of the data for on-line querying and analysis. Increasingly, however, we are seeing business intelligence applications in telecommunications, electronic commerce, and other industries, that are characterized by very high data volumes and data flow rates, and that require continuous analysis.
In this paper, then, we describe a few approaches that are being developed, including virtual data warehouses or enterprise portals that support access through views or links directly to the operational data sources. In this architecture, data flows continuously into a data warehouse, and is staged into one or more OLAP tools that are used as computation engines to continuously and incrementally build summary data cubes, which might then be stored back in the data warehouse. Analysis and data mining functions are performed continuously and incrementally over these summary cubes. Retirement policies define when to discard data from the warehouse 

**The key features of the architecture are the following:**
- Incremental data reduction using OLAP engines to generate summaries and enable data mining; staging large volumes and flow rates of data with different life spans at different levels of aggregation and scheduling operations on data depending on the type of processing to be performed and the age of the data.


# Introduction:
## what is data warehouse ?


**Data warehouse modeling is the process of building a model for the data that is to be stored in the data warehouse. The model produced is an abstract model, and in this sense, it is a representation of reality, or at least a part of reality which the data warehouse is assumed to support.** A Data Warehouse (DW) is a relational database that is designed for query and analysis rather than transaction processing. It includes historical data derived from transaction data from single and multiple sources. A Data Warehouse provides integrated, enterprise-wide, historical data and focuses on providing support for decision-makers for data modeling and analysis. 
A Data Warehouse can be viewed as a data system with the following attributes:
* It is a database designed for investigative tasks, using data from various applications.
* It supports a relatively small number of clients with relatively long interactions.
* It includes current and historical data to provide a historical perspective of information.
* Its usage is read-intensive.
* It contains a few large tables.

"Data Warehouse is a subject-oriented, integrated, and time-variant store of information in support of management's decisions."


## data warehousing 

- Data warehousing is the act of **Organizing** & **Storing** data in a way so as to make its retrieval efficient and insightful.
- It's also called as the process of transforming **data** into **information** 

	Data warehousing implements **the process to access heterogeneous data
	sources, clean, filter, and transform the data and store the data in a structure that is easy to access, understand, and use**. The data is then used for query,reporting, and data analysis. As such, the access, use, technology, and performance requirements are completely different from those in a transaction-oriented operational environment. The volume of data in data warehousing can be very high.


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
1. Data architecture modeling consists of a combination of top-down enterprise data modeling techniques and bottom-up (detailed) model integration. Data architecture modeling also should provide the techniques for logical data partitioning, granularity modeling, and building multitiered data architectures.

# Conclusion

Data house is not new phenomenon. All large organization already have data warehouses but they are not just managing them. Over the next few years , the growth of data is going to be enormous with new products and technologies coming out frequently. In order to get the most out of the period , it is going to important that data warehouse planners and devlopers have a clear idea of what they are looking for and then choose strategies and methods that will provide them with performance today and flexibility for tomorrow.  


# References 
1. http://ilpubs.stanford.edu:8090/76/1/1995-10.pdf

1. http://eddyswork.synthasite.com/resources/Data%20Modeling%20Tech%20For%20Data%20Warehouseing.pdf

1. https://www.youtube.com/watch?v=CHYPF7jxlik&t=355s

1. https://www.slideshare.net/KarthikSrini2/data-warehousing-71815590

1. https://www.researchgate.net/profile/Deepak-Sharma-119/publication/358675111_A_Study_on_Inventory_Management_System_A_Case_Study_of_Hindustan_Aeronautics_Limited_HAL_Nashik/links/620e8f4bf02286737ca61984/A-Study-on-Inventory-Management-System-A-Case-Study-of-Hindustan-Aeronautics-Limited-HAL-Nashik.pdf#page=41


