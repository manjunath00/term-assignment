# Term-assignment

**Assignment given by the mentor to explain the given terms with not more than 2 lines.**


## 10 popular commands - daily use

**1.** **touch** : It is used to modify the 'access time' & 'modification time'.  To modify only "access time" use "-a" option and to modify only "modification time" use "-m". If a **file doesn't exist** it creates a new file with that name. So, touch command **can be used to create a new file**.


```bash
touch filename #creates a new file, if doesn't exist
touch -a filename # modify only the access time
touch -m filename # modify only the modification time
touch -c filename # prevent creation of new file, if it doesn't exists
```

**2.** **mkdir** : It is used to create a new "directory" (folder).  you can pass in **-p** option to create whole path, if the parent folder doesn't exists.

```bash
mkdir foldername # creates a new folder/directory
mkdir -p parentfolder/childfolder # create folder 'parentfolder' if it doesn't exits.
```
**3.** **cd** : cd (change directory ) is used to switch between directories. **cd ..** will take you to one directory up. **cd -** will take you previous directory that you came from. **~** represents home directory. So, **cd ~** will take you to **home** directory.

```bash
# consider structure ~/homework/math/, you are in ~(home)
cd homework # get into homework folder
cd math # get into math folder
cd .. # go one directory up i.e. homework
cd - # takes you to last directory you were in i.e. math
```
**4.** **rm** : It is a command to remove file and folder. Once the file is deleted. you cannot easily recover the file. To remove folders you can -d option. To delete the **write protected** files it will ask for you prompt and to avoid prompt use **-f** option and to delete files recursively use **-r** option. Use option **-i** for prompt to appear before delete a file.

**NOTE:** **NEVER** use ```rm -rf``` in home directory with **ROOT** permissions.
```bash
# delete using rm command
rm homework.md # delete the file
rm file.txt file2.txt  # delete multiple files.
rm -i fib.py  # to ask before deleting. (prompt) hit 'y' to delete
rm -d folder # delete folders
rm -rf node_modules # delete files recursively and force fully
```
**5.** **mv** : It is used to move files and rename files. You can move multiples files to directory. to move files/folders you have first specify **source** and then **destination**. you can take backup before overwriting a files using -b option.

```bash
# delete using rm command
mv source_folder destination_folder # move the folder to a new folder
mv oldname.txt newname.txt  # rename using mv command
mv file1.txt file3.txt file2.txt dest_folder  # move multiple files to a folder.
mv file1.txt another_folder/file1.txt # overwrite to a file.
mv -b file1.txt file2.txt # backup of file1.txt will created before overwriting(renaming) to file2.txt
mv  -S .bak -b file1.txt file2.txt # -S to specify the extension of the backup file that you want.

```

**6.** **ls** : used to list the files and directories in the current directory.  **-a** lists all the files and folder i.e. hidden files and folder too. **-h** lists file sizes in human readable format. **-F** appends **/** at the end of the directories. **-R** lists files recursively inside all sub-directories (returns a very long list). **-ltr** option will list latest files first.  **-S** list files according to size in descending order.

```bash
# delete using rm command
ls  # lists files and folders inside the current folder
ls -l  # list files and folder with size, permission and other details
ls -a server_files  # list all (including hidden ones) files and folder in the given folder
ls  -lh # -h option will display size in human readable form.
ls -F  # appends "/" at the end of folder names while listing
ls  -R  # -R list all the files and folders inside the "sub-directories" inside the current folder.
ls -ltr # lists all the files in reverse time order (latest first) -r option to display in reverse.
ls -lS # -S with l with display size in descending order(biggest first)
```

