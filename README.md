# Oracle-Database-Lab-PDB-and-OEM-Configuration
Oracle PDB and OEM Configuration
Student Information

Name: Amos Nkurunziza
Student ID: 26973
Course: PL/SQL and Oracle Database Administration
Assignment Title: Oracle PDB and OEM Configuration
Date: 5/10/2025

1. Overview of Tasks

This report summarizes the Oracle practical exercises focused on creating, managing, and monitoring pluggable databases using Oracle Database 21c Express Edition. The tasks were divided into three main activities:

Task 1: Create a new Pluggable Database (PDB)

Task 2: Create and delete a PDB

Task 3: Configure and access Oracle Enterprise Manager (OEM)




2. Task 1: Creating a New Pluggable Database (PDB)

A new pluggable database was created using the following name:

plsql_class2025db


The username was generated based on the naming convention:

Amos_plsqlauca_26973


A simple password was used for authentication.
This database was successfully created and opened for use in classwork.

Screenshot:<img width="582" height="324" alt="TASK1" src="https://github.com/user-attachments/assets/6f33602b-ff40-457d-a770-3f558de91ed1" />
 PDB creation confirmation (attached).



3. Task 2: Creating and Deleting a PDB

For this task, another pluggable database was created following the format:

FirstTwoLettersOfName_to_delete_pdb_StudentID


Hence, the database name was:

am_to_delete_pdb_26973


After creating the PDB, it was successfully deleted to demonstrate proper lifecycle management.

Screenshot:<img width="706" height="301" alt="PDB TO DELETE" src="https://github.com/user-attachments/assets/be03e13c-0f98-4d6e-9502-9d054c8609d6" />
 Creation  confirmation (attached).
Screenshot:<img width="615" height="264" alt="PDB DELETION" src="https://github.com/user-attachments/assets/4c7eed17-f9a3-4947-8373-3d40ce881f86" />

 Deletion confirmation (attached).





4. Task 3: Oracle Enterprise Manager (OEM) Configuration

Oracle Enterprise Manager was accessed via:

https://localhost:5500/em


and logged in with administrative credentials.

The OEM dashboard displayed:

Database: XE (21.3.0.0.0 Express Edition)

Type: Single Instance (CDB with 1 PDB)

Metrics: CPU usage, memory allocation, and data storage

Schema visible: AMOS_PLSQ...

This confirms a successful configuration of OEM and database monitoring setup.

Screenshot:<img width="1887" height="930" alt="dashboard" src="https://github.com/user-attachments/assets/5ed379ba-1434-492f-a44b-52b1b8098dbd" />
 OEM Dashboard (attached).

5. Issues Encountered and Solutions
Issue	Cause	Solution
OEM not loading	Listener not started	Ran lsnrctl start
PDB not opening automatically	Database started in MOUNT mode	Executed ALTER PLUGGABLE DATABASE ALL OPEN;
Login failed	Wrong username/password	Re-entered correct credentials
6. Conclusion

All three tasks were successfully completed. The configuration demonstrates knowledge of Oracle container databases, pluggable database creation and deletion, and performance monitoring via OEM.
This hands-on exercise reinforced practical Oracle administration concepts.
