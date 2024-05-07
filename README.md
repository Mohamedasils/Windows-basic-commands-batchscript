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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

mkdir %userprofile%\Desktop\MyLab


![image](https://github.com/Mohamedasils/Windows-basic-commands-batchscript/assets/144870445/551dd0ed-000c-4832-9bb6-3424eeb90752)



## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.

cd %userprofile%\Desktop\MyLab




![image](https://github.com/Mohamedasils/Windows-basic-commands-batchscript/assets/144870445/65031b58-9a06-48bd-a6ec-e0490c225960)




![image](https://github.com/Mohamedasils/Windows-basic-commands-batchscript/assets/144870445/5175cd40-7aaa-41ca-908f-facb1d3f5ce1)



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.


dir %userprofile%\Desktop\MyLab



![image](https://github.com/Mohamedasils/Windows-basic-commands-batchscript/assets/144870445/d84fed66-18ae-4925-830c-338b46f21263)



## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/Mohamedasils/Windows-basic-commands-batchscript/assets/144870445/388ad639-8e9f-4dc7-8811-be679db8fb56)



## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents

![image](https://github.com/Mohamedasils/Windows-basic-commands-batchscript/assets/144870445/bbb7f8a1-5ebf-4115-9475-b5fb87f51de6)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```

@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!



```

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!

```



## OUTPUT

![image](https://github.com/Mohamedasils/Windows-basic-commands-batchscript/assets/144870445/4e3da1d0-1e79-43d5-a975-41394ce28bbb)




# RESULT:
The commands/batch files are executed successfully.

