# JupyterHub

## What is JupyterHub?

The Jupyter notebooks mentioned above are used in conjunction with JupyterHub. The term JupyterHub refers to the infrastructure set up on \[datahub.berkeley.edu\]\([http://datahub.berkeley.edu\](http://datahub.berkeley.edu\)\). This site provides cloud-based internet storage for assignments. Instructors and students can work on and store assignments entirely through JupyterHub. It is essentially the equivalent of Google Drive for Jupyter notebooks.

## Do you need JupterHub to use notebooks?

You don't need to use JupyterHub in order to use the Jupyter notebooks. Notebooks can be used and stored locally in your computer's filesystem. This requires some extra installation and setup that we have not provided directions for on this site. You don't need an internet connection in order to use and access the notebooks on your own computer. You do need an internet connection in order to use the \[datahub.berkeley.edu\]\([http://datahub.berkeley.edu\](http://datahub.berkeley.edu\)\) JupyterHub.

## Why does JupyterHub exist?

Working on JupyterHub ensures that all students and instructors are using the same computing environment, reducing installation or compatibility issues that come up with different computers and operating systems. In addition, the work stored over the cloud can be accessed from anywhere. Students who don't have access to a personal computer can still access their work through library computers.

## Getting Access

Anyone with a berkeley.edu email address has access to the JupyterHub at datahub.berkeley.edu. If anyone \(instructors, CAs, students\) is having trouble logging in, please make sure that the correct URL and a berkeley.edu email are being used for login. Please post on Piazza if you are unable to solve JupyterHub access issues.

## Pre-installed Python Packages

Many Python packages have been pre-installed on JupyterHub and are available to students by default. You can find of these pre-installed packages \[here\]\([https://github.com/data-8/connector-instructors/wiki/Python-Packages\#pre-installed\](https://github.com/data-8/connector-instructors/wiki/Python-Packages#pre-installed\)\). You can also \[install other packages\]\([https://github.com/data-8/connector-instructors/wiki/Python-Packages\](https://github.com/data-8/connector-instructors/wiki/Python-Packages\)\) that are not on this list.

## Technical Overview

JupyterHub is a cluster \(set of connected computers\) and each node \(computer\) in the cluster has several CPUs and a finite amount of memory. Each student also has disk space on JupyterHub. When people go to \[datahub.berkeley.edu\]\([http://datahub.berkeley.edu\](http://datahub.berkeley.edu\)\), JupyterHub will create an instance of Python + all class materials, and will reserve a CPU for them to run code. There are ~8 CPUs for each node, and they are shared by all the users currently logged-in to that node. Each user instance has roughly \*\*1 CPU, 10GB storage, and 2GB memory\*\*.

## CPU Restrictions

While CPU will restrict how fast your code runs, it's usually not the bottleneck on the cluster. Obviously you want to limit the complexity of the analyses you'd like students to run, and a good rule of thumb is to try and simplify analyses / datasets, and then discuss how they'd be scaled up. For example, running simple machine learning on in-memory data is probably fine. Fitting a multi-layer neural network on multiple batches of data is probably going to take a long time.

One thing that will tie up resources is running commands that request multiple CPUs. \*\*Please avoid using parallel computing in your code\*\* \(e.g., \`joblib\`, or \`n\_jobs &gt; 1\` in \`scikit-learn\`\). If you really want to do this, contact us on \[Piazza\]\([https://piazza.com/berkeley/other/cs97\](https://piazza.com/berkeley/other/cs97\)\) and we will try to set up something that works for you.

## Memory Restrictions

Currently there is 2GB for each student's session \(though this may be different in future iterations\). \*In the top-right  corner of notebooks you will find the amount of memory currently used out of the total amount available to students.\*

### What if I run out of memory?

* If you run out of memory, the python kernel will automatically restart.\*\* This can be frustrating for students because they don't get any kind of message that tells them memory is the problem. It's a good idea to let them know ahead of time.
* If restarting the kernel and re-running the code doesn't help, then usually there is another notebook open from a previous session. Go to the "running notebooks" page, and close anything you're not using right now.
* If all other notebooks are closed and you're \*still\* running out of memory, then log out and log back in to your JupyterHub account. This will close your session and then start a new one. There have been reports of stray memory being taken up by Python even though processes have finished running.



