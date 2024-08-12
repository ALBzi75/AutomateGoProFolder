# AutomateGoProFolder
Explanation:
Filtering and Deleting Files:

The script uses os.listdir() to list all files in the directory and filters those with extensions .LRV or .THM.
- os.remove() is used to delete the filtered files.
- Grouping Files by Modification Date:

The script iterates over the files, using os.path.getmtime() to get the last modification time, which is then formatted to dd.MM.yyyy.
- Files are grouped by this modification date.
- Creating Folders and Moving Files:

For each group, a folder is created (if it doesn't exist) using os.makedirs().
- Files are then moved into the corresponding folder using shutil.move().
This Python code should be run in an environment where you have the necessary permissions to delete and move files.
