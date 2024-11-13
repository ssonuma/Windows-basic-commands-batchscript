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
```mkdir %userprofile%\Desktop\MyLab```
![image](https://github.com/user-attachments/assets/411acf4c-623b-45e5-8667-8b576440ff8c)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```cd %userprofile%\Desktop\MyLab```
![image](https://github.com/user-attachments/assets/db05998d-df3e-4246-8d41-2a6c5e46406a)
![image](https://github.com/user-attachments/assets/6c60175d-3352-436d-925b-762c619757d0)



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```dir %userprofile%\Desktop\MyLab```
![image](https://github.com/user-attachments/assets/c0a5fe90-157c-4365-9113-705bd1ca9e4a)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/97892d88-6467-4bf6-bbcd-9df361486082)
![image](https://github.com/user-attachments/assets/9163cfd2-f755-42b7-8682-c890d0ae3549)


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![image](https://github.com/user-attachments/assets/d56047a0-df76-4f1c-a088-c6e198313e44)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```@echo off
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
![Uploading Screenshot 2024-11-13 110627.png…]()




# RESULT:
The commands/batch files are executed successfully.

