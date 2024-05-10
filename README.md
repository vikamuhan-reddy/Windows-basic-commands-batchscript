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


## COMMAND

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab
cd %userprofile%\Desktop\MyLab
type nul > MyFile.txt

```

## OUTPUT:
![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/50e9474a-648f-4e4d-b04d-7993d764d2d8)




## COMMAND

List the contents of the "MyLab" directory.
```
dir %userprofile%\Desktop\MyLab
```

## Output:
![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/e33ddd8a-3b19-444e-8937-54c1575f8f03)




## COMMAND

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

Move the "MyLab" directory to the "Documents" folder.

```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup

```


## OUTPUT
![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/381be0fe-5560-49f5-a262-50022d82ad84)




## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup

```
## OUTPUT:
![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/65784087-5c69-4a90-a803-6cc0c22ed868)



```
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx

```

## OUTPUT:
![image](https://github.com/vikamuhan-reddy/Windows-basic-commands-batchscript/assets/144928933/df69b616-dfe8-4eec-9f11-555dbbc92eeb)


# RESULT:
The commands/batch files are executed successfully.

