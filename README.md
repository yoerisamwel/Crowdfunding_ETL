# Crowdfunding_ETL
Project 2

## Project Goals:
This is a course project assignment from BCS to be completed as a team where the team is tasked to perform the Extract, Transform, and Load (ETL) process using <code>Jupyter Notebook</code>. The team members are <a href="https://github.com/rrrrasha">Ms. Abdalla</a>, <a href="https://github.com/drkrenn">Mr. Krenn</a>, <a href="https://github.com/123noob1">Mr. Ngo</a>, and <a href="https://github.com/yoerisamwel">Mr. Samwel</a>.

## Data Sources Files:
The key files for this project are in two locations within this repository. 
The first location is in the main folder of the repository. The file "ETL_Mini_Project_RAbdalla_DKrenn_KNgo_YSamwel.ipynb" contains all of the syntax used to extract, clean, manage, and analyze the data for this project. There's also "INSERT FILE NAME" in this folder which shows the entity relationship diagram (ERD) for the project. Finally, there's a SQL schema file named crowdfunding_db_schema.sql.
The second key location is in the "Resources" which contains 5 key excel files for the project. 

## Data Extraction & Cleaning: 
The data were imported from crowdfunding.xlsx. From there, the category & subcategory column was separated into a category column and a subcategory column. Then the unique values from category and subcategory were each exported into their own dataframe, and each item was assigned its own variable ID. The dataframes were then exported to separate excel files. 
In the next portion of the assignment, the main excel file, crowdfunding.xlsx, was cleaned and updated. A few variables were renamed with cleaner column headers. For a few of the columns, data types were updated, including the reformatting some columns as dates. The category and subcategory IDs were then imported in from the prevously created excel files. Columns that weren't needed were dropped, and the resulting dataframe was reexported to crowdfunding.xlsx. 
In the next portion of the assignment, a new dataframe was created to hold data on contacts. The original contacts spreadsheet had the data formatted as json. So the json data was imported and converted into a multicolumn dataframe. The dataframe was then cleaned and expored back into an excel file. Even though we were only required to do this processes using one of two approaches, we ultimately completed this portion using both techniques. 
The final portion of the project ties all of the previously created spreadsheets together. In order to make sense of all the data collectively, an ERD was created to show the cross-over constructs amongst all of the excel files. A database schema was created for SQL, and the data were loaded into a database named crowdfunding_db.
