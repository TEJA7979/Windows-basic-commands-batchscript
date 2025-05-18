# Ex08-Windows-basic-commands-batchscript

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
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/46879a6b-01ab-4c9e-84f4-de16bda9746b)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/9f3f1ed4-b355-4b08-b471-ab6a6f81efb6)

type nul > MyFile.txt

![image](https://github.com/user-attachments/assets/7a1b0924-fab3-4488-a155-3b29007e4dc7)


List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/e2a98080-3a42-4dde-b33e-a30c09f16e3b)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/df73be65-6a8c-40e3-9e98-39066c379c93)

copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/user-attachments/assets/b3b61c51-8a9c-4b66-b668-be67c998813d)


Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
```
![image](https://github.com/user-attachments/assets/ff8d7ba9-20c7-4d71-a6bf-ba820c40c22b)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

## OUTPUT
![image](https://github.com/user-attachments/assets/063d581e-0fbe-491a-8a98-f7246c5d044c)



# RESULT:
The commands/batch files are executed successfully.
