# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-22 173933](https://github.com/user-attachments/assets/b835f379-ca62-4136-9b5b-6400a7fb93ea)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-22 174130](https://github.com/user-attachments/assets/3a37b190-3842-402f-a0f2-81333294a993)

```
type nul > MyFile.txt
```
![Screenshot 2025-05-22 174303](https://github.com/user-attachments/assets/23d09ab2-a668-4fce-a81e-2e925b88556c)
List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-22 174407](https://github.com/user-attachments/assets/c3df738a-ebd4-42e2-9c8f-600854e06855)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Backup
```
![Screenshot 2025-05-22 174519](https://github.com/user-attachments/assets/bde2ea62-3373-49ce-8fb6-a33f0d0919d4)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2025-05-22 174557](https://github.com/user-attachments/assets/d2a7eed8-6c1c-43c4-a304-85eeb3551d05)

Move the "MyLab" directory to the "Documents" folder

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Documents
```
![Screenshot 2025-05-22 174721](https://github.com/user-attachments/assets/31f025d4-2193-47c5-a082-eb773e4db1c3)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
![Screenshot 2025-05-22 174856](https://github.com/user-attachments/assets/9ebd60c8-f480-4cbe-bf55-0cbb391af16e)

# RESULT:
The commands/batch files are executed successfully.

