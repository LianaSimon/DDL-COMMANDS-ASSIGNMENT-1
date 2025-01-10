# Comprehensive Guide to Using DDL Commands on a STUDENT Table in SQL

(DDL-COMMANDS-ASSIGNMENT-1)
Create a database named School and perform all the DDL commands (CREATE, ALTER, DROP, RENAME, TRUNCATE) for the table named STUDENT with fields: Roll_No Name Marks Grade Create data on your own based on the given columns

## SCRIPT

-- ASSIGNMENT 1-DDL COMMANDS

-- CREATE A DATABASE NAMED SCHOOL AND USE IT
CREATE DATABASE SCHOOL;
USE SCHOOL;

-- CREATE A TABLE NAMED STUDENT
CREATE TABLE STUDENT(
Roll_no INT PRIMARY KEY,
Full_name VARCHAR(50),
Marks INT,
Grade CHAR(1)
);

-- INSERT SAMPLE DATA INTO STUDENT TABLE
INSERT INTO STUDENT(Roll_no,Full_name,Marks,Grade)
VALUES(1,'SHRIYA SHARMA',96,'A'),(2,'KRISHNA NATH',85,'B'),(3,'DISHA RAJ',68,'C'),(4,'RISHAB KUMAR',75,'B'),(5,'SANYA SINGH',94,'A');

-- USE THE SELECT COMMAND TO DISPLAY THE TABLE
SELECT * FROM STUDENT;

-- ADD A COLUMN NAMED 'CONTACT' TO THE STUDENT TABLE.
ALTER TABLE STUDENT ADD Contact VARCHAR(15);
SELECT * FROM STUDENT;

-- REMOVE GRADE COLUMN FROM THE STUDENT TABLE
ALTER TABLE STUDENT DROP COLUMN GRADE;
SELECT * FROM STUDENT;

-- CHANGE THE NAME OF THE TABLE STUDENT TO CLASSTEN
ALTER TABLE STUDENT RENAME TO CLASSTEN;

-- DELETE ALL ROWS FROM THE CLASSTEN TABLE
TRUNCATE TABLE CLASSTEN;
SELECT * FROM CALSSTEN;

-- REMOVE THE CLASSTEN TABLE FROM THE DATABASE
DROP TABLE CLASSTEN;

## MYSQL WORKBENCH SNAPS OF SCRIPT AND EXECUTION

# Step 1: Create a database named School
![image](https://github.com/user-attachments/assets/b3a496fa-e1df-4771-aa95-1770d0ca1ad6)

# Step 2: Switch to the School database
![image](https://github.com/user-attachments/assets/80192f8c-da88-420a-8c3d-00c5121b8dc2)

# Step 3: Create a table named STUDENT
![image](https://github.com/user-attachments/assets/9fc72ca8-d163-4412-b232-6bb0e805e199)

# Step 4: Insert sample data into the STUDENT table
![image](https://github.com/user-attachments/assets/a7bfe60d-1c4a-4002-908d-acb2498236b1)

# Step 5: Use the SELECT command to display the table
![image](https://github.com/user-attachments/assets/d12a196c-9889-4b21-87db-6008c36c51d8)

# Step 6: Add a column named Contact to the STUDENT table
![image](https://github.com/user-attachments/assets/af64d8f4-e020-41e6-a355-1110f4dac89a)

# Step 7: Remove the Grade column from the STUDENT table
![image](https://github.com/user-attachments/assets/dee0d9d5-4252-4626-a865-20f41ad8ac32)

# Step 8: Rename the table to CLASSTEN
![image](https://github.com/user-attachments/assets/6df2a8c5-d5dc-4449-bc13-b4221b5f84dd)

# Step 9: Delete all rows from the CLASSTEN table
![image](https://github.com/user-attachments/assets/63fdfecb-b950-453a-9a74-cbb4f12eef90)

# Step 10: Remove the CLASSTEN table from the database
![image](https://github.com/user-attachments/assets/a4ecb550-fe0e-4eae-b5d6-83db10df255e)


# Summary of Commands and Actions:

*CREATE DATABASE: Creates the School database.
*CREATE TABLE: Creates the STUDENT table with specified fields.
*ALTER TABLE: Adds and removes columns, renames the table.
*TRUNCATE TABLE: Deletes all rows without logging individual row deletions.
*DROP TABLE: Deletes the table schema and data permanently.
*SELECT: Displays data from the table.

## Notes
Make sure the database does not already exist before running the script to avoid conflicts.
Review the script carefully and customize it as needed for your requirements.

## Contributing
Feel free to submit issues or pull requests to improve this script. Contributions are always welcome!

## Contact
For any questions or support, please contact lianasimon77@gmail.com
