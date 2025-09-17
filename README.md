# Snowflake_End_To_End_Data_Modelling

## Project Overview  
This project demonstrates an end-to-end ETL/ELT pipeline on Snowflake using cricket ODI JSON data. It covers data ingestion, staging, transformation, data modeling (fact & dimension tables), automation with tasks, and visualization in Snowsight.

---

## Key Steps  

1. **Loading JSON Data into Snowflake Stages**  
   - Uploaded JSON files from local machine to Snowflake internal stage.  
   - Queried staged files using `$` notation and ingested them into raw tables with `COPY INTO`.  

   ### 📸 Screenshot 1: Checking Data from JSON  
   *(Example of querying raw JSON data in Snowflake stage)*
   <img width="1280" height="726" alt="image" src="https://github.com/user-attachments/assets/2c4da839-9e65-4d7c-90a7-0f7d28d38f14" />


---

2. **Transforming Semi-Structured Data**  
   - Applied `FLATTEN()` function to handle nested JSON arrays and objects.  
   - Created staging tables and then designed Fact & Dimension tables using star schema.  

   ### 📸 Screenshot 2: Using `FLATTEN()` Function  
   *(Example of expanding nested JSON into relational form)*
   <img width="1280" height="718" alt="image" src="https://github.com/user-attachments/assets/f7aa9288-ef89-4877-ada8-fd06693ecf9c" />


