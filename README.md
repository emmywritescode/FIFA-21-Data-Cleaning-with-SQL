# FIFA 21 DATA CLEANING WITH SQL
![](intro.jng)
## Introduction
This project demonstrates the power and capabilities of SQL in performing data-cleaning tasks. SQL is specifically designed for working with databases and large datasets. It provides efficient query processing, making it well-suited for handling substantial amounts of data during the cleaning process. SQL queries are also explicit and reproducible. By saving and documenting the cleaning steps as SQL scripts, one can easily repeat the process on new data or share the cleaning workflow with others.

As a participant of the data cleaning challenge organized by Victor Somadina and Promise Chinonso, I had previously completed this task with Microsoft Excel but I wanted to put my SQL skills to the test as well.
## About the data set
The data set used was obtained from [Kaggle](https://www.kaggle.com/datasets/yagunnersya/fifa-21-messy-raw-dataset-for-cleaning-exploring). It contains various attributes and statistics of players in the popular video game FIFA 21, such as player ratings, skill moves, preferred positions, and more. The data set consists of 18,979 rows and 77 columns of data.
## The purpose of data cleaning
The purpose of data cleaning, also known as data cleansing or data scrubbing, is to improve the quality and reliability of data by identifying and correcting or removing errors, inconsistencies, and inaccuracies. Data cleaning is an essential step in the data preparation process and plays a crucial role in ensuring the accuracy and integrity of data for analysis, reporting, and decision-making purposes.
## The data cleaning process
### Importing the data set
The csv file was carefully imported into Microsoft SQL Server Management Studio using the SQL Server Import and Export Wizard. To eliminate the problem of character encoding plaguing the data set, the 'code page' was changed from '1252 (ANSI Latin-I)' to '65001 (UTF-8)' on the wizard's dialog box. The data type of the columns was also changed to the 'Unicode string'.
### Retreiving the table information
The stored procedure 'sp_help' was used to get a quick summary of the data set. This provided details such as the columns in the table, their data types, any indexes or constraints defined on the table, and other relevant information about the structure of the table.
 Code                  |     Output
:---------------------:|:---------------------:
  ![](table_info.png)  | ![](table_result.png) 
