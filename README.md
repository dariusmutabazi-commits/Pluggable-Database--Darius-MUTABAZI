# Pluggable-Database--Darius-MUTABAZI
## Assignment Report: Oracle Database 19c Practical Tasks
## Task 1: Create a New Pluggable Database (PDB)
I logged in to Oracle Database as SYSDBA and created a new pluggable database following the required format. After creating the PDB, I opened it successfully and confirmed that it was active. I then used the SHOW PDBS command to verify that the new PDB appeared in the list of available databases.
![image alt](https://github.com/dariusmutabazi-commits/Pluggable-Database--Darius-MUTABAZI/blob/main/creating%20first%20prugable%20database.PNG)        
**fig 1:** creating first pruggable database


![image alt](https://github.com/dariusmutabazi-commits/Pluggable-Database--Darius-MUTABAZI/blob/main/checking%20p%20database%201.PNG)        
**fig 2:** verifying if the pruggable database is created

## Task 2: Create and Delete a PDB
I created another pluggable database named da_to_delete_pdb_28239. After the creation, I opened the PDB and confirmed that it was running correctly using the SHOW PDBS command. Once verified, I closed the PDB using the ALTER PLUGGABLE DATABASE CLOSE IMMEDIATE command and then deleted it completely using DROP PLUGGABLE DATABASE da_to_delete_pdb_28239 INCLUDING DATAFILES. Finally, I confirmed that the PDB had been removed by running SHOW PDBS again.

![image alt](https://github.com/dariusmutabazi-commits/Pluggable-Database--Darius-MUTABAZI/blob/main/creation%20of%20another%20prugable%20database.PNG)       
**fig 3:** creation of pruggable database da_to_delete_pdb_28239

![image alt](https://github.com/dariusmutabazi-commits/Pluggable-Database--Darius-MUTABAZI/blob/main/verification%20of%20pdb1.PNG)        
**fig 4:** checking if it is really created

![image alt](https://github.com/dariusmutabazi-commits/Pluggable-Database--Darius-MUTABAZI/blob/main/closing%20the%20altered%20prugable%20database%20and%20deletion.PNG)     
**fig 5:** closing and deletion of pruggable database

![image alt](https://github.com/dariusmutabazi-commits/Pluggable-Database--Darius-MUTABAZI/blob/main/verification%20of%20pdb%202.PNG)       
**fig 6:** verifying if it has been deleted

## Task 3: Oracle Enterprise Manager (OEM) Dashboard
I opened Oracle Enterprise Manager in my browser and logged in using the SYS account. The dashboard displayed my username and the list of databases clearly. I confirmed that the OEM connection was working and captured a screenshot showing the system dashboard and my account details.
![image alt](https://github.com/dariusmutabazi-commits/Pluggable-Database--Darius-MUTABAZI/blob/main/OEM.PNG)         
**fig 7:** Oracle Enterprise Manager dashboard

## Issues and Fixes
During the exercise, I encountered the error ORA-65005, which occurred because the FILE_NAME_CONVERT clause was missing the source and target file paths. I corrected it by including both paths in the statement. I also faced the error ORA-65025 while dropping the PDB, which happened because the PDB was still open. I solved this by closing the PDB first with the ALTER PLUGGABLE DATABASE CLOSE IMMEDIATE command before dropping it.
## Result and short summary
All required tasks were completed successfully. I created, opened, verified, and deleted pluggable databases without further errors. I also accessed Oracle Enterprise Manager and confirmed my account information on the dashboard. The entire setup worked correctly and met all given requirements.
