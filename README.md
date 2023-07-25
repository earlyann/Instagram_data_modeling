## Instagram Data Modeling - Star Schema

### Project Overview
The Instagram Data Modeling project emphasizes the utilization of the star schema to structure a comprehensive and organized data model. This model encompasses user data, photos, interactions, and more, all extracted from Instagram. The core objective of this initiative is to transform and pipeline this data into a database. This facilitates easier access and better structure, enables scaling, and lays a solid foundation for any future analytics or performance enhancements regarding Instagram data.

The primary data source is comprised of generated data and sourced from Kaggle: (https://github.com/earlyann/instagram_database/assets/119711479/0db1218c-9e8c-4ec5-9a47-b4179d7bdae2). 

### Data Source
The data utilized in this project is fictional, sourced from the link above.

### Benefits of Data Transformation (CSVs to DB)
These are a few of the reasons why I chose to transform my data before any analysis. 
- Data Persistence: Assures data longevity, allowing historical data access.
- Data Integrity: Reduces the risk of errors via enforced constraints.
- Scalability: Handles large data sets and is able to grow effectively.
- Efficient Data Retrieval: Optimized for quick data access.
- Security: Features like access control and encryption keep data safe.
- Collaboration: Facilitates data sharing among users.
- Tool Integration: Easily integrates with analytical tools.
- Business Questions to Address

##### Why Choose Star Schema?
When exploring the data, I decided that this was a good candidate for star schema modeling. Here are a few benefits of the star schema:
- Simplicity: Easily understandable structure with a single fact table and connected dimension tables.
- Efficient Query Performance: Minimizes joins for data retrieval, speeding up performance.
- Scalability: Adaptable model that allows for the addition of new dimensions or facts.
- Business-Oriented: Aligned with business needs and analytical processes.
- Aggregation Support: Efficiently handles aggregations, especially in large data scenarios.
- Tool Integration: Compatible with many BI and data visualization tools.

### Schema Description
The star schema for the Instagram data consists of the following tables:
- interactions table: Central table connecting users, photos, tags, comments, likes, and follows via foreign key columns.
- users table: Contains data about Instagram users.
- photos table: Houses data on Instagram photos.
- likes table: Details about likes on photos.
- comments table: Contains data about comments on photos, including emoji usage and hashtag count.
- follows table: Data about following relationships between users.
- tags table: Info about tags used in comments.

![Screen Shot 2023-07-25 at 12 17 06 PM](https://github.com/earlyann/instagram_database/assets/119711479/69ca630d-fb43-419e-a362-e579bd271d05)

### Project Components
- A notebook for creating a PostgreSQL database - to create this database you must have PostGres installed and your own connection data entered into the notebook
- A notebook for crafting an SQLite database - only Python libraries are needed to create this
- The actual SQLite file.
  
### Technologies Used
- PostgreSQL
- SQLite
- SQLAlchemy

### Conclusion
The Instagram Data Modeling project delivers valuable insights into user behavior, engagement metrics, and content trends. By utilizing a star schema, the data model ensures organized storage, streamlined analysis, and potent insights into Instagram analytics. This project demonstrates the power of relational database design in driving business intelligence.

### Next Steps
I will include a Tableau notebook using my database.

Author: Lacey Morgan
