# Chinook-Symphony-Transforming-Data-into-Sales-Insights
# Overview:
- This repository presents a dimensional data model transformation of the Chinook sample database, representing a digital media store.  Chinook data model represents a digital media 
store, including tables for artists, albums, media tracks, invoices and customers. It adheres to data warehousing and data analysis best practices, enabling efficient querying, reporting, and visualization.

# Data Model Design:
! [dim_image] (https://github.com/Adityam0208/Chinook-Symphony-Transforming-Data-into-Sales-Insights/blob/main/Dimensional%20Model/Dim%20data%20model.png)
# Facts:
- FactInvoiceLine: Stores transaction-level details for invoice lines, including quantity, price, and customer information.
- Additional custom facts can be incorporated for specific analysis needs.
  
# Dimensions:
- DimCustomer: Captures customer demographics and attributes.
- DimEmployee: Represents employee information and reporting hierarchies.
- DimInvoice: Provides context for invoice headers, such as date, total amount, and payment method.
- DimArtist, DimAlbum, DimTrack: Describe music-related details, including media type and genre.
- DimDate: Provides time-based dimensions for granular analysis.
- DimCalendar: Supports various calendar-related calculations and hierarchies.

  
# Slowly Changing Dimensions (SCDs):
- Appropriate SCD types (Type 1, Type 2, or Hybrid) are implemented to handle changes in dimension attributes over time, ensuring data integrity and historical analysis.
  
# Surrogate Keys:
- Surrogate keys are utilized in all dimensions to decouple them from natural keys, simplifying maintenance and preventing referential integrity issues.
  
# Foreign Keys:
- Relationships between dimensions and facts are established using foreign keys, enabling efficient data retrieval and analysis.
  
# Source-to-Target Mappings:
- Clear mappings are defined between source tables and target dimensional tables, ensuring data accuracy and consistency.

# Implementation:
1. ER/Studio Data Architect:
- Created a visual representation of the dimensional data model within the ER modeling tool for clarity and documentation.

2. Generated DDL, Created Tables, Uploaded Data:
- Generated Data Definition Language (DDL) scripts to create the dimensional tables in various target databases (SQL Server, MySQL, PostgreSQL, Oracle 11g).
- Successfully uploaded data from the Chinook sample database into the respective target databases.

3. Power BI Visualization and Dashboards:
- Developed interactive reports and dashboards within Power BI, leveraging the dimensional model for insightful data exploration and analysis.
- The visualizations explore various aspects of the data, including:
  Customer buying behavior
  Artist and album performance
  Sales trends over time
  Other business-specific metrics
- You can find interactive versions of these visualizations in the powerbi folder of this repository.

4. Further Development:
- Consider incorporating additional custom dimensions and facts based on specific analytical needs.
- Explore more advanced data visualization techniques and tools.
