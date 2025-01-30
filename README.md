# File-Explorer-using-python
This script aims to organize files into folders based on their file type

## Steps Taken
1. **Import Required Libraries**  
   - I started by importing the necessary libraries.
   - The os module to allow me to check if files or folders exist, list files in a directory, and create new folders.
   - And the shutil module  to move files from one location to another.
   

2. **Define the Main Directory Path**  
   - Next, I specified the path of the folder where all the files are located.

3. **Create a List of Folder Names**  
   - I created a list containing the names of the subfolders where the files will be sorted. Each folder corresponds to a specific file type. For example a folder for CSV files.

4. **Check and Create Folders if They Don't Exist**  
   - I then looped through the list of folder names and checked if each folder already exists in the main directory. If a folder did not exist, I created it. This ensures that all necessary subfolders are set up before moving any files.

5. **Get a List of Files in the Directory**  
   - I retrieved a list of all files and folders inside the main directory. This allows me to go through each item and determine if it needs to be moved.
   
6. **Loop Through Each File**  
   - I then looped through each item in the directory and checked whether it was a file or a folder. This step ensures that only files are processed, preventing errors when attempting to move a folder.
   
7. **Identify File Type and Destination Folder**  
   - For each file, I checked its extension to determine where it should be moved.
   - If the file was a CSV file, it needed to go into the CSV folder.
   - If the file was an image (JPG, PNG), it needed to go into the image folder.
   - If the file was a text file, it needed to go into the text folder.
   - If the file type didn’t match any of these categories, it was left in the main directory.
     
8. **Move the File to the Correct Folder**  
   - After identifying the correct folder, I generated the destination path for the file. Before moving the file, I checked whether a file with the same name already existed in the destination folder. If the file did not already exist, I moved it to the appropriate subfolder.


