# ArcGIS-Professional-Application
Add-In's created for the ArcGIS Pro App

This repository contains projects which demonstrate the follow:
* Use of the ArcGIS Pro SDK
* Use Click Events and StreamReader/Writer objects
* All code written in C# using Visual Studio.

**Usage:**
  
   Can be installed using Visual Studio to run the .sln project.
    
**Purpose:**

    Allows customers to load folder connections into a new project.
    Resolved the inconvenience where folder connections are 
    project-specific.
    
**Work Flow:**

   Simply uses the Pro SDK to open a "create file" dialog box,
   reads each folder connection in your current project, and
   writes those folder locations to the text file. Loading
   a text file parses the input line-by-line and makes a new
   connection to each directory.
    
**Input:**

   1. Open ArcGIS Pro and either a new or existing Project.  
   2. Create a new Folder Connection in the Project window.

   ![UI](Folder-Connections-Manager/Images/FolderConnect.png)
   3. Click the "Save Connections" button in the "Folder Connection Manager" 
   Add-In pane. The current Folder Connection's will be saved as a list 
   in the text file.  
   4. Remove the Folder Connection you just created by right-clicking on it in 
   the Project window and selecting "Remove".

   ![UI](Folder-Connections-Manager/Images/RemoveFolder.png)  
   5. Load your saved Folder Connection by clicking the "Load Connection" button 
   in the "Folder Connection Manager" Add-In pane. Select the text file you 
   saved in step three.  
   6. Verify that your Folder Connection has returned to the Project.  
    
**Output:**

   Creates a file (of your prefered extension) which is essentially
   a text file where each row containsa a different folder name.
