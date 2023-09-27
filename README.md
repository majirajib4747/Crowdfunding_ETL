For the ETL mini project, you will work with a partner to practice building an ETL pipeline using Python, Pandas, and either Python dictionary methods or regular expressions to extract and transform the data. After you transform the data, you'll create four CSV files and use the CSV file data to create an ERD and a table schema. Finally, you’ll upload the CSV file data into a Postgres database.

Since this is a one-week project, make sure that you have done at least half of your project before the third day of class to stay on track.

Although you and your partner will divide the work, it’s essential to collaborate and communicate while working on different parts of the project. Be sure to check in with your partner regularly and offer support.

- Main file:-  ETL_Project_2_Team_3.ipynb contains all the code to clean up the Excel files and import into CSV ( Which been used for database creation). 

- Explanation:- Initially we extracted all the data from crowdfunding.xlsx
Then, created a category and subcategory DataFrame that has the following columns:
* A "category_id" and Òsubcategory_id column that is numbered sequential form 1 to the length of the number of unique categories and subcategories.
* A "category" column that has only the categories and a ÒsubcategoryÓ column that has only the subcategories.
* Exported the DataFrame as aÊ  category.csv and Êsubcategory.csv .
Next, Created a Campaign DataFrame that has the  cf_id ,contact_id ,company_name, blurb column is renamed as description, goal and pledged column is converted to a float datatype, backers_count, country, currency, launched_at  column is renamed as launch_date and converted to a datetime format, deadline column is renamed as end_date and converted to a datetime format, category_id and subcategory_id with the unique number matching the category_id  and subcategory_id from the category and subcategory DataFrame. create a column that contains the unique four-digit contact ID number from theÊcontacts.xlsx
Then export the DataFrame as aÊcampaign.csv

Also, Create a Contacts DataFrame that has a column named "contact_id" that contains the unique number of the contact person, column named "first_name" that contains the first name of the contact person , acolumn named "last_name" that contains the first name of the contact person and a column named "email" that contains the email address of the contact person
Then export the DataFrame as aÊcontacts.csv
-  QuickDBD-Crowdfunding_DB_Schema.sql contain create table Queries and basic select queries for all 4 Tables.

Sketched an ERD of the tables , to create a table schema for CSV files. Also, specify the data types, primary keys, foreign keys, and other constraints.
![QuickDBD-crowdfunding](https://github.com/majirajib4747/Crowdfunding_ETL/assets/137097511/3d2a5664-38de-445a-8682-f2cc697b17b3)





- Resource Folder :- contains all the original Excel Files and csv file created through Jupyter Notebook.


