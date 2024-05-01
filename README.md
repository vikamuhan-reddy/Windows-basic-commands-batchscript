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

![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/e7cb1f11-8652-40a1-b7c8-0a65e5e9a177)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab

![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/4a20d7c8-5836-4263-b713-657a2dd66c4f)
![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/82ef2564-e2c5-49ce-903d-e99c15216825)

List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab

![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/6af7a87d-cba0-473e-ac1b-5b403efb9ea8)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/29608159-c9ae-43ab-8ab1-52c41182a62c)
![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/9006e802-f9fd-4818-ab09-45c9edf4c7c1)


Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents

![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/7365b8b7-66eb-44b1-af94-e3b1fc291a88)


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
![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/41f9b3ca-598d-4335-b268-436d415830d2)


# RESULT:
The commands/batch files are executed successfully.

