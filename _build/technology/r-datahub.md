---
interact_link: content/technology/r-datahub.ipynb
kernel_name: ir
has_widgets: false
title: 'R DataHub'
prev_page:
  url: /technology/pedagogy-and-technology/notebook-zero.html
  title: 'Notebook Zero'
next_page:
  url: /connector/instructor/logistics.html
  title: 'Logistics, Rooms, and Technology'
comment: "***PROGRAMMATICALLY GENERATED, DO NOT EDIT. SEE ORIGINAL FILES IN /content***"
---
# Introduction to Datahub for R

## What is Datahub?

Datahub ([datahub.berkeley.edu](https://datahub.berkeley.edu)) is a cloud-based computing platform maintained by UC Berkeley. It runs on JupyterHub to create, store, distribute, and manage scripts, datasets, and related files. Anyone with a UC Berkeley email is able to access Datahub - there are no additional set-up steps for affiliated students and faculty.

Courses teaching R are encouraged to use [r.datahub.berkeley.edu](https://r.datahub.berkeley.edu) for instructional infrastructure. Materials can easily be distributed to students by using an interact link (described below). Instructors will set up a web link that automatically pulls files into student accounts from a public Github repo. 

Datahub also supports connections to grading platforms such as [okpy.org](https://okpy.org) and [gradescope.com](https://gradescope.com). With proper integration, students will be able to automatically submit assignments to these platforms for instructors to view and grade in real time.

## Workflow

In designing course materials for use on datahub, there are four steps in the typical workflow

1. Create assignments using R or RMD files on your local desktop. 
2. Publishing assignments to a public Github repo when they are ready to be released.
3. Create an interact link to published assignment
4. Distribute the interact link for students to use to access course materials
5. Determine appropriate submission instructions for students.

## Set-Up

<ol>
<li>On Github, create two new repositories

<ul>
<li>One private repository should contain all course materials. This will include any assignments, datasets, images, solutions, set-up materials, and .RProj files that are relevant to your course. (ex. `phw250fg-dev`)</li>
<li>One public repository should contain all materials that have been published to students for a specific term. This will be continuously updated through the course of the semester. Only put files here if you want students to have access to them (ex. don’t include solutions) (ex. `phw250fg2019`)</li>
</ul>
</li>
<li>On your computer, create a new folder to hold all course materials (both published and unpublished)
<ul>
<li>Clone both of the repos from above into this folder
<ul>
<li>See Appendix A for a quick guide to git, including repo cloning</li>
</ul>
</li>
</ul>
</li>
<li>Your file set-up should now look something like this:

<pre>	PHW250FG
       ↳ phw250fg-dev (folder for all materials)
       ↳ phw250fg2019 (folder for materials published to students)
</pre>
</li>
</ol>

### Assignment Creation

All assignment creation should take place in the folder designated for the development of course material (ex. `phw250fg-dev`). To ensure that working directories are properly set, create an `.RProj` file within the folder. 

We recommend that you use RStudio to create `.R` or `.Rmd` file templates. If needed, add the appropriate data files to the folder as well. When loading data, set paths relative to the base level of the folder (where the `.RProj` file was created). The here package is a good tool for making sure your file paths are correct.

For PHW250FG, the development folder structure is as follows:
<pre>PHW250FG
   ↳ phw250fg-dev.RProj (project file used to set correct working directories)
   ↳ data (contains all data that is used throughout the course)
   ↳ setup
    ↳ autograder-setup (contains autograder files for all assignments)
        ↳ hw0-autograder (contains autograder files for homework 0)
        ↳ hw1-autograder (contains autograder files for homework 1)
        ↳ ...
   ↳ homework (contains blank student copies for assignments)
    ↳ hw0 (contains blank student copy of homework 0)
    ↳ hw1 (contains blank student copy of homework 1)
    ↳ …
   ↳ solutions (contains copies for assignments with solutions)
    ↳ hw0-solutions (contains solutions for homework 0)
    ↳ hw1-solutions(contains solutions for homework 1)
    ↳ …
</pre>

### Publishing Assignments

To publish assignments, relevant files must be copied from the development repository to the student materials repository. This can be done manually through a file explorer by copying files from one folder to the other, or automatically through a shell script (see Appendix B). Once the files have been copied to the student assignment repository, make sure to commit and push your changes (see Appendix A).

### Distributing Assignments

To distribute materials to students, you must create an interact link. This can be done through JupyterHub’s interact link generator. 

Fill out the fields as follows:

* JupyterHub URL - [ttps://r.datahub.berkeley.edu](https://r.datahub.berkeley.edu)
* Github Repository URL - URL of your public student materials repository, e.g. [https://github.com/UCB-Epi-R/phw250fg2019](https://github.com/UCB-Epi-R/phw250fg2019)
* Branch - master
* File to open - leave empty; functionality to automatically load a particular file for students is not currently available for r.datahub (as of August 2019)
* Application to Open - RStudio

At this point, your custom interact link appears at the top of the page. Copy this and link send to students. When this link is clicked, the materials in the public student repository will copied to their datahub accounts.

### Viewing Student Progress

Datahub allows instructors to access the datahub accounts of students and view files in their working environment. To do this, instructors must be added as admins on r.datahub This can be done by opening up a Github issue with the DataHub infrastructure team here. 

To view an individual student’s work:

* View the admin control panel at [https://r.datahub.berkeley.edu/hub/admin](https://r.datahub.berkeley.edu/hub/admin)
* Find the student’s CalNet username
* If necessary, click on “Start Server”
* Click on “Access Server”





## Appendix A: Introduction to Github

Github ([https://github.com/](https://github.com/)) is an online platform that allows you to share and collaborate on code. It’s a great tool to use if you have multiple people developing assignments or need a secure place to store course material from semester to semester.

### Creating a Repository

After signing-in/creating an account, navigate to [https://github.com/new](https://github.com/new). Fill out the repository name and description. Select public/private depending on the type of repo you’re making (for course materials, select public for student-facing materials and private for instructor-facing materials). Select “Initialize this repository with a README”. After filling out this page, you’ll be taken to the site that your repository is hosted on.

### Cloning a Repository

To work on the content of the repo on your computer, you must clone the repository by following these instructions:

1. Go to the github page for your repo. Click the green button labeled “Clone or download”. Copy the url that pops up
2. On your desktop, navigate to the folder where you want the repo to be copied to
3. Open a terminal within this folder
4. Type in `git clone GITHUB_URL` replacing `GITHUB_URL` with the url that you copied in step 1.
5. At this point, your repo has been cloned to your local desktop. You can add/edit/delete files in the repo folder as you would any other folder.
   
### Adding and Committing Changes

After making edits to the contents of your local copy of the repo, you must commit changes before they can be published to the repo stored online. Follow these instructions to add and commit your changes:

1. On your desktop, navigate to the folder containing your repo.
2. Open a terminal within the repo folder
3. Type in `git status`, which will show you all the changes you have made since you last pulled or cloned the repo. Make note of which files you want to publish publicly or for other collaborators to see.
4. For each file that you want to publish, type in `git add FILE_NAME` replacing `FILE_NAME` with the name of the relevant file.
5. Once you have added all of the files you needed,  type in `git commit -m “MESSAGE”` replacing `MESSAGE` with a description of the changes that were made

### Pushing Changes

After you have committed your changes, you must push them to GitHub before collaborators and students can view the updated files. To push, type `git push` in the terminal. 

## Appendix B: Introduction to Shell Scripts

Shell scripts are set of Unix commands that are written to a file and run sequentially when the file is executed. It is used to automate repetitive tasks and keep track of commands that must be run for a particular task.

To create a shell script:

1. Open a text editor, save the file as a `FILENAME.sh` (ex: publish.sh)
2. Type in `#!/bin/bash` at the head of the document. This indicates the the contents below are part of a bash script.
3. For each item or folder that you want copied, add a line with the following format. Replace `SOURCE_FILEPATH` with the relative file path to the file(s) you want to copy and `DEST_FILEPATH` with the relative path to the folder where you want the file(s) to be copied 

```bash
cp- -r [SOURCE_FILEPATH] [DEST_FILEPATH]
```

For PHW250FG, the shell script is saved as publish.sh and is located at the root level of the development repository. The contents are as follows:

```bash
#!/bin/bash

#Copy all data
cp -r data ../phw250fg2019

#Update with new assignment names
cp -r setup/autograder-setup/hw1_r_quiz/ ../phw250fg2019/setup/autograder-setup/
cp -r homework/hw1_r_quiz/ ../phw250fg2019/homework/
```

 
