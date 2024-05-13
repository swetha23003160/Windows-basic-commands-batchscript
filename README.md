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
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

![image](https://github.com/23002027/Windows-basic-commands-batchscript/assets/139752981/9502cfa4-b01c-41be-b9c7-495f7c17be77)





## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
List the contents of the "MyLab" directory.


![image](https://github.com/23002027/Windows-basic-commands-batchscript/assets/139752981/8751423e-f46a-4ab1-8659-bae4c9971315)
![image](https://github.com/23002027/Windows-basic-commands-batchscript/assets/139752981/94fb3869-2d36-4fa6-8383-32685b249b57)




## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLabCopy "MyFile.txt" to a new folder named "Backup" on the desktop.
![image](https://github.com/23002027/Windows-basic-commands-batchscript/assets/139752981/013f4945-16e6-499f-a10e-6fd95ba59c21)






## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
Move the "MyLab" directory to the "Documents" folder.
![image](https://github.com/23002027/Windows-basic-commands-batchscript/assets/139752981/9764c92a-f692-471c-8d8e-c160621e0b3f)
![image](https://github.com/23002027/Windows-basic-commands-batchscript/assets/139752981/71f85cef-e8f3-4134-8a00-4489c6b7a1e0)



## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![image](https://github.com/23002027/Windows-basic-commands-batchscript/assets/139752981/d867d801-3115-4e21-8f99-a7bb80cfa591)





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
![image](https://github.com/23002027/Windows-basic-commands-batchscript/assets/139752981/c95d5c31-e72d-4f3f-924e-19ce123d48b9)





# RESULT:
The commands/batch files are executed successfully.

