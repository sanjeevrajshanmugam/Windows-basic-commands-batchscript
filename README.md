# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

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

## COMMAND AND OUTPUT


mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/sanjeevrajshanmugam/Windows-basic-commands-batchscript/assets/151383137/5b31d133-af08-4778-8511-6245efb2d9bd)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab
![image](https://github.com/sanjeevrajshanmugam/Windows-basic-commands-batchscript/assets/151383137/076a23a3-867d-4da6-a949-dbec07516e9f)
type nul > MyFile.txt
![image](https://github.com/sanjeevrajshanmugam/Windows-basic-commands-batchscript/assets/151383137/c5fd5116-416c-49b2-bef2-2200a061b9c0)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab
![image](https://github.com/sanjeevrajshanmugam/Windows-basic-commands-batchscript/assets/151383137/5bc1a4ef-c8d1-4089-ac2c-f0dede2fe678)



Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup
![image](https://github.com/sanjeevrajshanmugam/Windows-basic-commands-batchscript/assets/151383137/32a7b550-f1c3-4989-8366-9477144402ee)
copy MyFile.txt %userprofile%\Desktop\Backup



Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Documents
move MyLab Documents
![image](https://github.com/sanjeevrajshanmugam/Windows-basic-commands-batchscript/assets/151383137/d8dad433-0349-4d55-85e3-c9058531e234)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!

![image](https://github.com/sanjeevrajshanmugam/Windows-basic-commands-batchscript/assets/151383137/58b1bf3c-aefb-42dd-8862-0579194ca4b9)

@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!

![image](https://github.com/sanjeevrajshanmugam/Windows-basic-commands-batchscript/assets/151383137/9159da54-56d3-4699-acee-c778e3b3ad1b)














# RESULT:
The commands/batch files are executed successfully.

