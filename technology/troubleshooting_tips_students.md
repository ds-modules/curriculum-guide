# Tips to Use Datahub

## About the UC Berkeley DataHub:  

The DataHub is UC Berkeley’s implementation of Jupyterhub and is a free service made available to UC Berkeley students to provide a small amount of computing and storage on a virtual machine running in the cloud. This guide provides an overview of the tasks you will need to complete before the semester begins, during the semester, and at the end of the semester. This high-level information will help you navigate your coursework effectively using the UC Berkeley DataHub.

#### Before the Semester Begins


##### 1. Browser and Internet Check

**Browser Compatibility:** Ensure you are using a compatible web browser (Chrome, Firefox, Safari) that is updated to the latest version.

**Internet Connection:** Verify you have a stable internet connection to access DataHub smoothly. 

##### 2. Account Setup and Access
**Activate CalNet ID:** Ensure your CalNet ID is activated and functioning properly.

**Access DataHub:** Go to datahub.berkeley.edu and log in with your CalNet ID to verify you can access the platform. (and allow bcourses to authenticate when you get the message “DataHub is requesting access to your account”.) 

##### 3. Familiarize Yourself with DataHub
**Overview:** Review student resources to understand the varied features of DataHub.

**Interface Tour:** Explore the DataHub interface, including the JupyterLab and RStudio environments.

#### During the Semester

##### 1. Accessing Course Materials
**Course Hub:** Use nbgitpuller links shared by your course instructors to launch notebooks in DataHub

**Notebooks and Scripts:** Open and work on Jupyter Notebooks, R scripts, or other files as provided by your instructor.

**To manage files in JupyterHub:** To upload a file, click the "Upload" button in the JupyterHub interface and select the file from your local machine.To download a file, right-click on the file in the JupyterHub interface and select the "Download" option.

##### 2. Completing Assignments
Regular Use: Regularly log in to DataHub to complete assignments, run analyses, and work on projects.
Save Work: Save your progress frequently. It's good practice to manually save your work as well.
Check Storage Space: Delete unnecessary files and constantly check the storage size of the home directory.  You can do this by opening a Terminal, and executing du -sh
Don’t Duplicate Shared Directory Content: If your course work requires shared directories where instructors are storing large datasets, don’t create a copy of the files in your home directory. Always, read data from the shared directory.
Do Your Work in Sub Directories: Create a sub directory for each assignment and do your work there. Avoid working on assignments from the root directory as they may lead to data issues if done wrongly.

##### 3. Collaboration and Sharing
```{note}
Datahub doesn’t have collaboration tools at this time as we are continuously testing the latest updates.
```

**Instructor Feedback:** Share your work with instructors or TAs for feedback by downloading and submitting your notebooks as required.

##### 4. Troubleshooting
**Restart Kernel/Server:** Try restarting your kernel as a classic troubleshooting step to see if the error goes away. If the problem persists, restart your server.
 
**Kill Process:** Having too many things open on Datahub can cause issues. Sharing two different approaches to check running processes and kill them,

**Option 1: UI Based Approach:**
- In Notebook - click Jupyter Icon in UR to get to ”tree” 
- In “tree” click running processes tab
- Right click on any process to kill it ( or Kill all). In Lab you can see running processes in tab on left with this icon

**Option 2: CLI approach:**
- Open the terminal in Datahub.
- Use the command ps aux to list all running processes.
- Find the process ID (PID) of the processes you want to stop.
- Use the command kill <PID> to terminate those processes.
- Repeat these steps as necessary to manage your system resources.

**Support:** Reach out to course TAs for technical help, and they will contact infrastructure staff if they are unable to resolve your issue.

What if I can’t access DataHub?
Ensure your CalNet ID is active and try logging in again. If the problem persists, inform your TA or check out this guide for additional help.
How do I install additional packages?
Use !pip install package-name in a Jupyter Notebook cell for Python packages, or install.packages("package-name") in the R console.


Can I use DataHub off-campus?
Yes, you can access DataHub from anywhere with an internet connection.
What should I do if I encounter a technical issue?
First, try restarting your kernel. If the issue persists, contact your course TA,  and if they can’t resolve it they will reach out to DataHub staff.

#### End of the Semester
##### 1. Backup Your Work

**Backup coursework:** Back up your notebooks and data to either your personal device or an external storage service like Google Drive, Dropbox.

**User Home Directory Archiving:** Files unused for 90 days will be archived and stored in a low cost storage. You will need to open a request with the DataHub team to retrieve your unused files.

##### 2. Clean Up Your Workspace
**Clean Up:** Clean up your DataHub workspace by deleting unnecessary files and folders.

**Feedback:** Provide feedback on your experience with the DataHub team to help improve the service for future students.