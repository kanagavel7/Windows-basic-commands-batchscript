# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript      
NAME:R.KANAGAVEL
REG.NO:212223040085

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

![Screenshot 2024-04-27 141517](https://github.com/kanagavel7/Windows-basic-commands-batchscript/assets/162578954/8456786b-1ed8-480e-aacc-93ab41042a0f)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![Screenshot 2024-04-27 141645](https://github.com/kanagavel7/Windows-basic-commands-batchscript/assets/162578954/7973d789-8f01-4527-b42f-da74d6552d01)

![Screenshot 2024-04-27 141654](https://github.com/kanagavel7/Windows-basic-commands-batchscript/assets/162578954/ad938e3a-f320-4e65-885c-9e32e8f3cfc0)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![Screenshot 2024-04-27 141749](https://github.com/kanagavel7/Windows-basic-commands-batchscript/assets/162578954/be8e013e-4994-4565-a73b-b9ce43c0694c)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![Screenshot 2024-04-27 141826](https://github.com/kanagavel7/Windows-basic-commands-batchscript/assets/162578954/9c6171d0-f751-4822-9c98-ef58a9f3f502)

![Screenshot 2024-04-27 141847](https://github.com/kanagavel7/Windows-basic-commands-batchscript/assets/162578954/484f088d-159b-4797-b758-1f63adf8249b)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![Screenshot 2024-04-27 142002](https://github.com/kanagavel7/Windows-basic-commands-batchscript/assets/162578954/eaf84db0-2d53-482d-96ee-4a1acfb78ce5)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT

![Screenshot 2024-04-27 142202](https://github.com/kanagavel7/Windows-basic-commands-batchscript/assets/162578954/6efec54d-5e29-4316-8982-98288dddc508)

# RESULT:
The commands/batch files are executed successfully.
