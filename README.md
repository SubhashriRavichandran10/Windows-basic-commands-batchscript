# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

## NAME : R.SUBHASHRI
## REGISTER NO : 212223230219

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.

  mkdir %userprofile%\Desktop\MyLab
  
  
  
  ![image](https://github.com/SubhashriRavichandran10/Windows-basic-commands-batchscript/assets/145743413/893365db-c185-455b-9bb1-ab0452e7ae76)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
  

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.

cd %userprofile%\Desktop\MyLab


![image](https://github.com/SubhashriRavichandran10/Windows-basic-commands-batchscript/assets/145743413/481fed75-c6a1-46f4-868b-a6691553a3ba)


![image](https://github.com/SubhashriRavichandran10/Windows-basic-commands-batchscript/assets/145743413/a8378773-3c1a-4887-9c76-07f124c65ac3)






## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.


dir %userprofile%\Desktop\MyLab


![image](https://github.com/SubhashriRavichandran10/Windows-basic-commands-batchscript/assets/145743413/e3d3a5e1-54ef-42c1-9c47-c7736eaaed16)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.


mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/SubhashriRavichandran10/Windows-basic-commands-batchscript/assets/145743413/c83cbc44-59ae-4e93-b484-88308ab1748e)


![image](https://github.com/SubhashriRavichandran10/Windows-basic-commands-batchscript/assets/145743413/1ea2d6a8-3e9a-4a49-85fc-faad209d7cdf)


## COMMAND AND OUTPUT


mv Myfile.txt %userprofile%\Documents


![image](https://github.com/SubhashriRavichandran10/Windows-basic-commands-batchscript/assets/145743413/b9e64d20-6358-44c6-8490-bdf95a1b9322)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!


Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.


@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!




## OUTPUT


![image](https://github.com/SubhashriRavichandran10/Windows-basic-commands-batchscript/assets/145743413/078f8fa9-aaae-4d97-a7df-190fbfe8569b)



# RESULT:
The commands/batch files are executed successfully.

